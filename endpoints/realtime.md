# Realtime

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

Query params: transport, clientProtocol, connectionToken, connectionData, _.

Starts the realtime notifications stream.

Response (captured):

    {
      "Response": "started"
    }

## POST /notifications/abort

Query params: transport, clientProtocol, connectionToken, connectionData.

Aborts the realtime notifications stream.

Response: not captured.

## WS /notifications/connect

Query params: transport, clientProtocol, connectionToken, connectionData, tid.

WebSocket for realtime notifications.

Response: not captured.
