
# System Notification Event Body

## Class Name

`SystemNotificationEventBody`

## Cases

| Type | Factory Method |
|  --- | --- |
| [`SystemAlertNotificationEvent`](../../../doc/models/system-alert-notification-event.md) | SystemNotificationEventBody.fromSystemAlertNotificationEvent(SystemAlertNotificationEvent systemAlertNotificationEvent) |
| [`SystemMaintenanceNotificationEvent`](../../../doc/models/system-maintenance-notification-event.md) | SystemNotificationEventBody.fromSystemMaintenanceNotificationEvent(SystemMaintenanceNotificationEvent systemMaintenanceNotificationEvent) |
| [`SystemPerformanceNotificationEvent`](../../../doc/models/system-performance-notification-event.md) | SystemNotificationEventBody.fromSystemPerformanceNotificationEvent(SystemPerformanceNotificationEvent systemPerformanceNotificationEvent) |

## SystemAlertNotificationEvent

### Initialization Code

#### Example

```java
SystemNotificationEventBody.fromSystemAlertNotificationEvent(
        new SystemAlertNotificationEvent.Builder(
            "system.alert"
        )
        .build()
    )
```

## SystemMaintenanceNotificationEvent

### Initialization Code

#### Example

```java
SystemNotificationEventBody.fromSystemMaintenanceNotificationEvent(
        new SystemMaintenanceNotificationEvent.Builder(
            "system.maintenance"
        )
        .build()
    )
```

## SystemPerformanceNotificationEvent

### Initialization Code

#### Example

```java
SystemNotificationEventBody.fromSystemPerformanceNotificationEvent(
        new SystemPerformanceNotificationEvent.Builder(
            "system.performance"
        )
        .build()
    )
```

