# Catalog

## GET /v1/catalog/metadata

Host: catalog.octane.wtf

Returns catalog feature flags.

Response (captured):

    {
      "numberOfCatalogItemsToDisplayOnSplash": 25,
      "numberOfCatalogItemsToDisplayOnSplashOnPhone": 15,
      "isCatalogSortsFromApiEnabled": false,
      "is3dInEachItemCardAbTestingEnabled": false,
      "is3dInEachItemCardEnabled": false
    }

## GET /v1/categories

Returns catalog categories as an object where values are category IDs.

Response (captured):

    {
      "Featured": 0,
      "All": 1,
      "Collectibles": 2,
      "Clothing": 3,
      "BodyParts": 4
    }

## GET /v1/subcategories

Same shape as categories.

Response (captured):

    {
      "Featured": 0,
      "All": 1,
      "Collectibles": 2,
      "Clothing": 3,
      "BodyParts": 4
    }

## GET /v1/search/navigation-menu-items

Returns menu items for the catalog.

Response: not captured.

## GET /v1/search/items

Host: catalog.octane.wtf

Searches catalog items.

Query params: category, subcategory, keyword, limit, maxPrice, minPrice, includeNotForSale.

Response (captured):

    {
      "_total": 2040,
      "keyword": null,
      "elasticsearchDebugInfo": null,
      "nextPageCursor": "60",
      "previousPageCursor": null,
      "data": [
        {
          "itemType": "Asset",
          "id": 410061
        }
      ]
    }

## GET /v1/recommendations/metadata

Returns recommendation metadata.

Response: not captured.

## POST /v1/catalog/items/details

Host: catalog.octane.wtf

Returns full details for a list of items.

Response (captured):

    {
      "data": [
        {
          "id": 399157,
          "assetType": 41,
          "name": "Blonde Messy Vkei Scene Emo Hair",
          "description": "",
          "genres": ["All"],
          "creatorType": "User",
          "creatorTargetId": 1,
          "creatorName": "Octane",
          "offsaleDeadline": null,
          "itemRestrictions": [],
          "saleCount": 13,
          "itemType": "Asset",
          "favoriteCount": 2,
          "isForSale": true,
          "price": 27,
          "priceTickets": null,
          "lowestPrice": null,
          "priceStatus": null,
          "lowestSellerData": null,
          "unitsAvailableForConsumption": null,
          "serialCount": 0,
          "moderationStatus": "ReviewApproved",
          "createdAt": "2026-10-25T20:10:18.846956Z",
          "updatedAt": "2026-10-25T20:14:03.58776Z"
        }
      ]
    }
