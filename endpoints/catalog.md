# Catalog

## GET /v1/catalog/metadata

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

Searches catalog items.

Query params: category, subcategory, keyword, limit.

Response: not captured.

## GET /v1/recommendations/metadata

Returns recommendation metadata.

Response: not captured.

## POST /v1/catalog/items/details

Returns full details for a list of items.

Response: not captured.
