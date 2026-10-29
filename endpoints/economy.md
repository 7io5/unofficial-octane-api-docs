# Economy

## GET /v1/users/{userId}/currency

Host: economy.octane.wtf

Returns a user's currency balances.

Response (captured):

    {
      "robux": 24,
      "tickets": 10
    }

## GET /apisite/economy/v1/users/{userId}/currency

Host: octane.wtf

Returns the authenticated user's currency balances.

Response (captured):

    {
      "robux": 24,
      "tickets": 65
    }

## GET /v1/users/{userId}/revenue/summary/day

Returns daily revenue summary for a user's games.

Response: not captured.

## GET /apisite/economy/v1/assets/{assetId}/resale-data

Host: octane.wtf

Returns resale data for an asset.

Response (captured):

    {
      "assetStock": 0,
      "sales": 0,
      "numberRemaining": 0,
      "recentAveragePrice": 0,
      "priceDataPoints": [],
      "volumeDataPoints": []
    }

## GET /apisite/economy/v1/assets/{assetId}/resellers

Host: octane.wtf

Query params: cursor, limit.

Returns resellers for an asset.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": []
    }

## POST /apisite/economy/v1/purchases/products/{productId}

Host: octane.wtf

Purchases a product.

Response (captured):

    {
      "purchased": true,
      "reason": "Success",
      "productId": 410241,
      "currency": 1,
      "price": 0,
      "assetId": 410241,
      "assetName": "Tux",
      "assetType": "T-Shirt",
      "assetTypeDisplayName": "T-Shirt",
      "assetIsWearable": true,
      "sellerName": "Sykk",
      "transactionVerb": "bought",
      "isMultiPrivateSale": false
    }

## GET /apisite/economy/v2/assets/{assetId}/details

Host: octane.wtf

Returns details for an asset.

Response (captured):

    {
      "TargetId": 410241,
      "AssetId": 410241,
      "ProductId": 410241,
      "Name": "Tux",
      "Description": "",
      "AssetTypeId": 2,
      "Creator": {
        "Id": 27233,
        "Name": "Sykk",
        "CreatorType": "User",
        "CreatorTargetId": 27233
      },
      "IconImageAssetId": 0,
      "Created": "2026-10-29T00:21:37.626958Z",
      "Updated": "2026-10-29T03:55:10.853342Z",
      "PriceInRobux": 0,
      "PriceInTickets": null,
      "Sales": 0,
      "IsNew": false,
      "IsForSale": true,
      "IsPublicDomain": true,
      "IsLimited": false,
      "IsLimitedUnique": false,
      "Remaining": 0,
      "MinimumMembershipLevel": 0
    }
