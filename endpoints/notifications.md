# Notifications

## GET /v2/notifications/get-settings

Returns the authenticated user's notification settings.

Response (captured):

    {
      "notificationBandSettings": [
        {
          "notificationSourceType": "Test",
          "receiverDestinationType": "DesktopPush",
          "isEnabled": true,
          "isOverridable": true,
          "isSetByReceiver": false,
          "pushNotificationDestinationPreferences": []
        }
      ],
      "optedOutNotificationSourceTypes": [],
      "optedOutReceiverDestinationTypes": []
    }

## GET /notifications/negotiate

Starts a realtime notifications connection.

Response: not captured.

## GET /notifications/start

Starts the realtime notifications stream.

Response: not captured.

## POST /notifications/abort

Stops an active notifications connection.

Response: not captured.
