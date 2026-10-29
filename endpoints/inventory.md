# Inventory

## GET /v1/users/{userId}/assets/collectibles

Host: inventory.octane.wtf

Returns collectible assets a user owns.

Query params: assetType, cursor, limit, sortOrder.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": [
        {
          "userAssetId": 1044290,
          "serialNumber": 101,
          "assetId": 398944,
          "recentAveragePrice": 246,
          "originalPrice": 35,
          "serialCount": null,
          "assetStock": 205,
          "assetTypeId": "Face",
          "name": "Red Fang"
        }
      ]
    }

## GET /v2/recommendations/{userId}

Returns inventory recommendations for a user.

Response: not captured.

## GET /v2/assets/{assetId}/owners

Host: inventory.octane.wtf

Returns the owner list for an asset.

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

## GET /apisite/inventory/v1/users/{userId}/items/Asset/{assetId}

Host: octane.wtf

Returns whether a user owns a specific asset.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": []
    }
