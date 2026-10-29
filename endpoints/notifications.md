# Notifications

## GET /v2/notifications/get-settings

Host: notifications.octane.wtf

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

Host: realtime.octane.wtf

Query params: clientProtocol, connectionData, _, connectionToken.

Negotiates a realtime notifications connection.

Response (captured):

    {
      "Url": "/notifications",
      "ConnectionToken": "4d063c7a-6cef-4bef-b99e-69ac69d1d573",
      "ConnectionId": "4d063c7a-6cef-4bef-b99e-69ac69d1d573",
      "KeepAliveTimeout": 20,
      "DisconnectTimeout": 30,
      "ConnectionTimeout": 110,
      "TryWebSockets": true,
      "ProtocolVersion": "1.5",
      "TransportConnectTimeout": 5,
      "LongPollDelay": 0
    }

## GET /notifications/start

Host: realtime.octane.wtf

Query params: transport, clientProtocol, connectionToken, connectionData, _.

Starts the realtime notifications stream.

Response (captured):

    {
      "Response": "started"
    }

## POST /notifications/abort

Host: realtime.octane.wtf

Query params: transport, clientProtocol, connectionToken, connectionData.

Stops an active notifications connection.

Response: not captured.

## WS /notifications/connect

Host: realtime.octane.wtf

Query params: transport, clientProtocol, connectionToken, connectionData, tid.

WebSocket connection for realtime notifications.

Response: not captured.
