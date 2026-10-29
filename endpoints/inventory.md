# Inventory

## GET /v1/users/{userId}/assets/collectibles

Returns collectible assets a user owns.

Query params: assetType, cursor, limit, sortOrder.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": [
        {
          "userAssetId": 981367,
          "serialNumber": null,
          "assetId": 348649,
          "recentAveragePrice": 113,
          "originalPrice": 20,
          "serialCount": null,
          "assetStock": 160,
          "assetTypeId": "Hat",
          "name": "Halloween Santa Hat"
        }
      ]
    }

## GET /v2/recommendations/{userId}

Returns inventory recommendations for a user.

Response: not captured.

## GET /v2/assets/{assetId}/owners

Returns the owner list for an asset. Hosted on inventory.octane.wtf.

Query params: limit, cursor.

Response (captured):

    {
      "nextPageCursor": "100",
      "previousPageCursor": null,
      "data": [
        {
          "owner": {
            "id": 5,
            "type": "User",
            "name": "Boma"
          },
          "id": 185424,
          "serialNumber": null,
          "created": "2026-09-30T18:17:51.374546Z",
          "updated": "2026-09-30T18:17:51.374546Z"
        }
      ]
    }
