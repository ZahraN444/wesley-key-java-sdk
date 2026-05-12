
# User Notification Event Body

## Class Name

`UserNotificationEventBody`

## Cases

| Type | Factory Method |
|  --- | --- |
| [`UserActionNotificationEvent`](../../../doc/models/user-action-notification-event.md) | UserNotificationEventBody.fromUserActionNotificationEvent(UserActionNotificationEvent userActionNotificationEvent) |
| [`UserStatusNotificationEvent`](../../../doc/models/user-status-notification-event.md) | UserNotificationEventBody.fromUserStatusNotificationEvent(UserStatusNotificationEvent userStatusNotificationEvent) |
| [`UserPreferenceNotificationEvent`](../../../doc/models/user-preference-notification-event.md) | UserNotificationEventBody.fromUserPreferenceNotificationEvent(UserPreferenceNotificationEvent userPreferenceNotificationEvent) |

## UserActionNotificationEvent

### Initialization Code

#### Example

```java
UserNotificationEventBody.fromUserActionNotificationEvent(
        new UserActionNotificationEvent.Builder(
            "user.action"
        )
        .build()
    )
```

## UserStatusNotificationEvent

### Initialization Code

#### Example

```java
UserNotificationEventBody.fromUserStatusNotificationEvent(
        new UserStatusNotificationEvent.Builder(
            "user.status"
        )
        .build()
    )
```

## UserPreferenceNotificationEvent

### Initialization Code

#### Example

```java
UserNotificationEventBody.fromUserPreferenceNotificationEvent(
        new UserPreferenceNotificationEvent.Builder(
            "user.preference"
        )
        .build()
    )
```

