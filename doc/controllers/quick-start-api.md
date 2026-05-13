# Quick Start API

```java
QuickStartAPIController quickStartAPIController = client.getQuickStartAPIController();
```

## Class Name

`QuickStartAPIController`

## Methods

* [Address Validation](../../doc/controllers/quick-start-api.md#address-validation)
* [Rate Request](../../doc/controllers/quick-start-api.md#rate-request)
* [Track Request](../../doc/controllers/quick-start-api.md#track-request)
* [Rate Shop](../../doc/controllers/quick-start-api.md#rate-shop)
* [Void Request](../../doc/controllers/quick-start-api.md#void-request)
* [Ship Request](../../doc/controllers/quick-start-api.md#ship-request)
* [Rate Request - International](../../doc/controllers/quick-start-api.md#rate-request---international)
* [Ship Request - International](../../doc/controllers/quick-start-api.md#ship-request---international)


# Address Validation

Address validation checks an address against a carrier's records. When used within the UI, typically in a shipping app under the Ship To tab, the VALIDATE button will return a VALID response if the check is good, or a popout box showing an updated address from the carrier which can then be accepted if desired.

The carrier in use by default for address validation can be assigned via the Administration App, under Carriers. On our test system, our default address validation carrier is set to FedEx Web Services (ID 49), as they have a robust database of addresses to check against. However, you can additionally test with another carrier by specifying the Carrier in the parameters below. Using Carrier ID 7, for instance, will use DHL XML-PI to perform the validation.

For more information on supported carriers and their IDs, please see the <a href="http://documentation.transtream.com/Content/Carriers/CarriersList.htm">All Carriers Matrix</a> reference.
Additionally, more information regarding the Address Validation can be found here: <a href="http://documentation.transtream.com/Content/AddressValidation/Introduction.htm">Address Validation</a>.

```java
CompletableFuture<PierbridgeAddressValidationResponse> addressValidationAsync(
    final PierbridgeAddressValidationRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`PierbridgeAddressValidationRequest`](../../doc/models/pierbridge-address-validation-request.md) | Body, Required | - |

## Response Type

**200**

[`PierbridgeAddressValidationResponse`](../../doc/models/pierbridge-address-validation-response.md)

## Example Usage

```java
PierbridgeAddressValidationRequest body = new PierbridgeAddressValidationRequest.Builder(
    "apitest",
    new Address.Builder(
        "1600 Pennsylvania Avenue NW",
        "Washington",
        "DC",
        "20500",
        "US"
    )
    .build()
)
.build();

quickStartAPIController.addressValidationAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```


# Rate Request

Running a rate request will send certain shipment parameters to the carrier to return expected charges. In many cases, this can be as simple as providing the receiver's address and some package details. When some details such as the sender's address is not specified, the system uses the shipping user's assigned location to determine the origin address. Other details can be omitted and will be included from the defaults already configured in the system defaults, allowing requests to be simple when default values will be sufficient. Additional details can be provided, however, by filling in further parameters below.

Some details that may be needed can include line item information for products contained in the package, content descriptions, or declared values. Additionally, special services can be included as well. For more information regarding carrier services, please see the <a href="http://documentation.transtream.com/Content/Carriers/SupportedCarriers.htm">Supported Carriers</a> reference.

This rate request is using Carrier 3 for UPS API and ServiceType 25 for UPS Ground.

```java
CompletableFuture<PierbridgeRateResponse> rateRequestAsync(
    final PierbridgeRateRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`PierbridgeRateRequest`](../../doc/models/pierbridge-rate-request.md) | Body, Required | - |

## Response Type

**200**

[`PierbridgeRateResponse`](../../doc/models/pierbridge-rate-response.md)

## Example Usage

```java
PierbridgeRateRequest body = new PierbridgeRateRequest.Builder(
    "apitest",
    3,
    25,
    new Receiver.Builder()
        .companyName("The White House")
        .street("1600 Pennsylvania Avenue NW")
        .city("Washington")
        .region("DC")
        .postalCode("20500")
        .country("US")
        .build()
)
.packages(new Packages.Builder(
        Arrays.asList(
            new Package.Builder()
                .receiverName("Mr President")
                .receiverPhone("202-456-1414")
                .packageType(11)
                .weight(10.5D)
                .length(7D)
                .width(8D)
                .height(9D)
                .contentDescription("A gift")
                .build()
        )
    )
    .build())
.build();

quickStartAPIController.rateRequestAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```


# Track Request

The track request uses a PackageID to query the package history and return a status. For testing purposes, a sample PackageID has been included here to test, however, as the shipment was performed as a test shipment, no valid tracking information is returned.

If you have performed a test shipment using the Ship Request endpoint, the response provided will contain a PackageID for that shipment that can be substituted here. Again, it will not return valid tracking info as it is a test shipment, but you can see how to simply process a shipment and then track it with the returned data.

```java
CompletableFuture<PierbridgeTrackResponse> trackRequestAsync(
    final PierbridgeTrackRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`PierbridgeTrackRequest`](../../doc/models/pierbridge-track-request.md) | Body, Required | - |

## Response Type

**200**

[`PierbridgeTrackResponse`](../../doc/models/pierbridge-track-response.md)

## Example Usage

```java
PierbridgeTrackRequest body = new PierbridgeTrackRequest.Builder(
    "apitest",
    new Packages10.Builder(
        Arrays.asList(
            new Package11.Builder()
                .packageID(1234)
                .build()
        )
    )
    .build()
)
.build();

quickStartAPIController.trackRequestAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```


# Rate Shop

A rate shop uses a pre-defined group of carriers and services to return rates for comparison. These rates can allow the user to review for a supported delivery date, a supported special service, or simply the best shipping price. Rate groups are configured in the Administration App under Carriers, and each has a specific ID associated with it for the purposes of performing a rate shop.

In our demo code here, we are using Rate Group 9, which is configured in the system to rate shop using several carriers for domestic Ground shipments. We have selected FedEx Web Services Home Delivery for residential, and FedEx Web Services Ground, UPS API Ground, and USPS Postage First-Class Mail as services to rate for non-residential. When the rate shop is performed, all valid rates will be returned for the shipment parameters provided.

As such, not every carrier/service will always return a valid rate when performing a rate shop. For example, as FedEx Ground and Home Delivery are meant to be used exclusively between residential or non-residential addresses, only one will return a valid rate if both selected in the rate group, based on the destination address's residential flag. They have been included for comparison purposes but may error if the address is not valid for the service.

Additionally, other parameters may come into play when obtaining a rate, such as weight limits or minimums, or supported origin/destination areas. Check with your carrier to verify what they accept and review the returned messages to see if any parameters are not supported.

```java
CompletableFuture<PierbridgeRateShopResponse> rateShopAsync(
    final PierbridgeRateShopRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`PierbridgeRateShopRequest`](../../doc/models/pierbridge-rate-shop-request.md) | Body, Required | - |

## Response Type

**200**

[`PierbridgeRateShopResponse`](../../doc/models/pierbridge-rate-shop-response.md)

## Example Usage

```java
PierbridgeRateShopRequest body = new PierbridgeRateShopRequest.Builder(
    "apitest",
    new Receiver2.Builder()
        .companyName("The White House")
        .street("1600 Pennsylvania Avenue NW")
        .city("Washington")
        .region("DC")
        .postalCode("20500")
        .country("US")
        .build()
)
.packages(new Packages3.Builder(
        Arrays.asList(
            new Package3.Builder()
                .weight(10.5D)
                .length(7D)
                .width(8D)
                .height(9D)
                .contentDescription("A gift")
                .build()
        )
    )
    .build())
.rateGroup(1)
.build();

quickStartAPIController.rateShopAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```


# Void Request

The void request uses a PackageID to void a previously produced shipment/label. For testing purposes, a sample PackageID has been included here to test, however, as the shipment was performed as a test shipment, the void request will respond that the record is not found.

If you have performed a test shipment using the Ship Request endpoint, the response provided will contain a PackageID for that shipment that can be substituted here. Using this ID in the void request will void the test shipment you previously produced.

```java
CompletableFuture<PierbridgeVoidResponse> voidRequestAsync(
    final PierbridgeVoidRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`PierbridgeVoidRequest`](../../doc/models/pierbridge-void-request.md) | Body, Required | - |

## Response Type

**200**

[`PierbridgeVoidResponse`](../../doc/models/pierbridge-void-response.md)

## Example Usage

```java
PierbridgeVoidRequest body = new PierbridgeVoidRequest.Builder(
    "apitest"
)
.packages(new Packages12.Builder(
        Arrays.asList(
            new Package13.Builder()
                .packageID(1234)
                .build()
        )
    )
    .build())
.build();

quickStartAPIController.voidRequestAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```


# Ship Request

The ship request is where the bulk of our processes are performed. This is where you provide the full shipment details to send to the carrier. Some shipments, such as domestic US ground shipments, require very little information to generate a label. Just as in the rate request, the system uses defaults already configured to fill in details when not provided. Further details can be provided, however, by filling in further parameters below.

Some details that may be needed can include line item information for products contained in the package, content descriptions, or declared values. Additionally, special services can be included as well. For more information regarding carrier services, please see the <a href="http://documentation.transtream.com/Content/Carriers/SupportedCarriers.htm">Supported Carriers</a> reference.

This ship request is using Carrier 3 for UPS API and ServiceType 25 for UPS Ground.

```java
CompletableFuture<PierbridgeShipResponse> shipRequestAsync(
    final PierbridgeShipRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`PierbridgeShipRequest`](../../doc/models/pierbridge-ship-request.md) | Body, Required | - |

## Response Type

**200**

[`PierbridgeShipResponse`](../../doc/models/pierbridge-ship-response.md)

## Example Usage

```java
PierbridgeShipRequest body = new PierbridgeShipRequest.Builder(
    "apitest",
    3,
    25,
    new Receiver4.Builder(
        "1600 Pennsylvania Avenue NW",
        "Washington",
        "DC",
        "20500",
        "US"
    )
    .companyName("The White House")
    .build()
)
.packages(new Packages6.Builder(
        Arrays.asList(
            new Package7.Builder()
                .receiverName("Mr President")
                .receiverPhone("202-456-1414")
                .packageType(11)
                .weight(10.5D)
                .length(7D)
                .width(8D)
                .height(9D)
                .contentDescription("A gift")
                .build()
        )
    )
    .build())
.build();

quickStartAPIController.shipRequestAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```


# Rate Request - International

This endpoint is the same as the Rate Request, but has been preset to rate a simple international shipment. The parameters needed are generally the same as for domestic rating, but for some carriers can require additional line item or customs detail.

For more information regarding carrier services, please see the <a href="http://documentation.transtream.com/Content/Carriers/SupportedCarriers.htm">Supported Carriers</a> reference.

This rate request is using Carrier 3 for UPS API and ServiceType 26 for UPS Worldwide Express.

```java
CompletableFuture<PierbridgeRateResponse> rateRequestInternationalAsync(
    final PierbridgeRateRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`PierbridgeRateRequest`](../../doc/models/pierbridge-rate-request.md) | Body, Required | - |

## Response Type

**200**

[`PierbridgeRateResponse`](../../doc/models/pierbridge-rate-response.md)

## Example Usage

```java
PierbridgeRateRequest body = new PierbridgeRateRequest.Builder(
    "apitest",
    3,
    26,
    new Receiver.Builder()
        .companyName("Prime Ministers Office")
        .street("10 Downing St")
        .city("London")
        .region("GB")
        .postalCode("SW1A 2AA")
        .country("GB")
        .build()
)
.packages(new Packages.Builder(
        Arrays.asList(
            new Package.Builder()
                .receiverName("Mr Prime Minister")
                .receiverPhone("+44-20-7925-0918")
                .packageType(11)
                .weight(10.5D)
                .length(7D)
                .width(8D)
                .height(9D)
                .contentDescription("A gift")
                .international(new International1.Builder()
                    .contents(new Contents.Builder(
                        Arrays.asList(
                            new Content.Builder()
                                .quantity(1D)
                                .value(10D)
                                .valueCurrency("USD")
                                .weight(10.5D)
                                .weightUOM("lb")
                                .description("Fancy Goods")
                                .originCountry("US")
                                .itemCode("1234")
                                .itemDescription("Fancy Goods")
                                .unitsOfMeasure("PCS")
                                .partNumber("1234")
                                .build()
                        )
                    )
                    .build())
                    .build())
                .build()
        )
    )
    .build())
.build();

quickStartAPIController.rateRequestInternationalAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```


# Ship Request - International

This endpoint is the same as the Ship Request, but has been preset to ship a simple international shipment. The parameters here have been increased to include the International and Content nodes that contain line item detail required for international shipments from most carriers.

For more information regarding carrier services, please see the <a href="http://documentation.transtream.com/Content/Carriers/SupportedCarriers.htm">Supported Carriers</a> reference.

This ship request is using Carrier 3 for UPS API and ServiceType 26 for UPS Worldwide Express.

```java
CompletableFuture<PierbridgeShipResponse> shipRequestInternationalAsync(
    final PierbridgeShipRequest body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`PierbridgeShipRequest`](../../doc/models/pierbridge-ship-request.md) | Body, Required | - |

## Response Type

**200**

[`PierbridgeShipResponse`](../../doc/models/pierbridge-ship-response.md)

## Example Usage

```java
PierbridgeShipRequest body = new PierbridgeShipRequest.Builder(
    "apitest",
    3,
    26,
    new Receiver4.Builder(
        "10 Downing St",
        "London",
        "GB",
        "SW1A 2AA",
        "GB"
    )
    .companyName("Prime Ministers Office")
    .build()
)
.packages(new Packages6.Builder(
        Arrays.asList(
            new Package7.Builder()
                .receiverName("Mr Prime Minister")
                .receiverPhone("+44-20-7925-0918")
                .packageType(11)
                .weight(10.5D)
                .length(7D)
                .width(8D)
                .height(9D)
                .contentDescription("A gift")
                .international(new International9.Builder()
                    .contents(new Contents6.Builder(
                        Arrays.asList(
                            new Content6.Builder()
                                .quantity(1D)
                                .value(10D)
                                .valueCurrency("USD")
                                .weight(10.5D)
                                .weightUOM("lb")
                                .description("Fancy Goods")
                                .originCountry("US")
                                .itemCode("1234")
                                .itemDescription("Fancy Goods")
                                .unitsOfMeasure("PCS")
                                .partNumber("1234")
                                .build()
                        )
                    )
                    .build())
                    .build())
                .build()
        )
    )
    .build())
.build();

quickStartAPIController.shipRequestInternationalAsync(body).thenAccept(result -> {
    // TODO success callback handler
    System.out.println(result);
}).exceptionally(exception -> {
    // TODO failure callback handler
    exception.printStackTrace();
    return null;
});
```

