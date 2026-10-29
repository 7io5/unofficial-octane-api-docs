# Trades

## GET /v1/trades/inbound

Host: trades.octane.wtf

Query params: cursor, limit, sortOrder.

Returns inbound trades.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": []
    }

## GET /v1/trades/outbound

Query params: cursor, limit, sortOrder.

Returns outbound trades.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": [
        {
          "id": 8597,
          "user": {
            "id": 19808,
            "name": "OCT",
            "displayName": "OCT"
          },
          "created": "2026-10-25T14:46:26.069677Z",
          "expiration": "2026-10-30T14:46:26.073077Z",
          "isActive": true,
          "status": "Open"
        }
      ]
    }

## GET /v1/trades/inactive

Query params: cursor, limit, sortOrder.

Returns old or finished trades.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": [
        {
          "id": 8604,
          "user": {
            "id": 13471,
            "name": "231",
            "displayName": "231"
          },
          "created": "2026-10-25T19:32:00.554273Z",
          "expiration": "2026-10-30T19:32:00.555539Z",
          "isActive": false,
          "status": "Declined"
        }
      ]
    }

## GET /v1/trades/completed

Query params: cursor, limit, sortOrder.

Returns completed trades.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": [
        {
          "id": 8172,
          "user": {
            "id": 3,
            "name": "dax",
            "displayName": "dax"
          },
          "created": "2026-10-19T19:18:19.262223Z",
          "expiration": "2026-10-24T19:18:19.26418Z",
          "isActive": false,
          "status": "Completed"
        }
      ]
    }

## GET /v1/trades/{tradeId}

Returns full details for one trade.

Response (captured):

    {
      "id": 8597,
      "user": {
        "id": 19808,
        "name": "OCT",
        "displayName": "OCT"
      },
      "offers": [
        {
          "user": {
            "id": 1043,
            "name": "Zyko",
            "displayName": "OnlyTwentyCharacters"
          },
          "userAssets": [
            {
              "id": 293498,
              "serialNumber": null,
              "assetId": 69930,
              "name": "Sinister Q.",
              "recentAveragePrice": 325,
              "originalPrice": 32,
              "assetStock": 140,
              "membershipType": "None"
            },
            {
              "id": 134397,
              "serialNumber": null,
              "assetId": 35236,
              "name": "Blizzard Beast Mode Bandana",
              "recentAveragePrice": 188,
              "originalPrice": 10,
              "assetStock": 302,
              "membershipType": "None"
            },
            {
              "id": 745738,
              "serialNumber": 12,
              "assetId": 205036,
              "name": "Horror Movie Reject",
              "recentAveragePrice": 107,
              "originalPrice": 20,
              "assetStock": 245,
              "membershipType": "None"
            },
            {
              "id": 828010,
              "serialNumber": null,
              "assetId": 221817,
              "name": "The Raven",
              "recentAveragePrice": 154,
              "originalPrice": 25,
              "assetStock": 225,
              "membershipType": "None"
            }
          ],
          "robux": null
        },
        {
          "user": {
            "id": 19808,
            "name": "OCT",
            "displayName": "OCT"
          },
          "userAssets": [
            {
              "id": 955915,
              "serialNumber": 9,
              "assetId": 338292,
              "name": "Emo King",
              "recentAveragePrice": 749,
              "originalPrice": 100,
              "assetStock": 69,
              "membershipType": "None"
            }
          ],
          "robux": null
        }
      ],
      "created": "2026-10-25T14:46:26.069677Z",
      "expiration": "2026-10-30T14:46:26.073077Z",
      "isActive": true,
      "status": "Open"
    }

## POST /v1/trades/send

Sends a trade request.

Response: not captured.

## POST /v1/trades/{tradeId}/decline

Declines a trade.

Response: not captured.

## GET /apisite/trades/v1/trades/inbound/count

Host: octane.wtf

Returns inbound trade count.

Response (captured):

    {
      "count": 0
    }

## GET /apisite/trades/v1/users/{userId}/can-trade-with

Host: octane.wtf

Checks whether the authenticated user can trade with a target user.

Response: not captured.
