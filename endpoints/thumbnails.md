# Thumbnails

## GET /v1/assets

Host: thumbnails.octane.wtf

Returns thumbnails for assets.

Query params: assetIds, format, size, returnPolicy.

Response (captured):

    {
      "data": [
        {
          "targetId": 492,
          "state": "Completed",
          "imageUrl": "https://tcdn.octane.wtf/23086666b0bb5c07b3b4deb02b22ed8bddc77f9b7538c4234d79987cbe14a066.png",
          "version": ""
        }
      ]
    }

## GET /apisite/thumbnails/v1/assets

Host: octane.wtf

Returns thumbnails for assets.

Query params: assetIds, format, size, returnPolicy.

Response (captured):

    {
      "data": [
        {
          "targetId": 410241,
          "state": "Completed",
          "imageUrl": "https://tcdn.octane.wtf/65e6506073309ccbc74e529cfefe3ea525f20ccc5bf1da94641681b08043f0ee.png",
          "version": ""
        }
      ]
    }

## GET /v1/badges/icons

Returns badge icons.

Response: not captured.

## GET /v1/games/icons

Returns game icons.

Response: not captured.

## GET /v1/games/multiget/thumbnail

Returns thumbnails for multiple games.

Response: not captured.

## GET /v1/groups/icons

Returns group icons.

Response (captured):

    {
      "data": [
        {
          "targetId": 548,
          "state": "Completed",
          "imageUrl": "https://tcdn.octane.wtf/3d69f2ea973a702cf6605ad066ccc3b0d6c7295d6d399f3212c24c79524de52d.png",
          "version": ""
        },
        {
          "targetId": 623,
          "state": "Completed",
          "imageUrl": "https://tcdn.octane.wtf/3f27c9e0c69b82f8cb8ff19c6f11612c6e0c01bf1a64d29a6a076a366a1bb46f.png",
          "version": ""
        }
      ]
    }

## GET /v1/places/gameicons

Returns place game icons.

Response: not captured.

## GET /v1/users/avatar

Returns full body avatar thumbnails.

Response (captured):

    {
      "data": [
        {
          "targetId": 1043,
          "state": "Completed",
          "imageUrl": "https://tcdn.octane.wtf/0412799a09373f3852b700370dfe795f937b766b44d4eaec71fab85a66f4f766_thumbnail.png",
          "version": ""
        }
      ]
    }

## GET /v1/users/avatar-headshot

Returns headshot thumbnails.

Response (captured):

    {
      "data": [
        {
          "targetId": 1043,
          "state": "Completed",
          "imageUrl": "https://tcdn.octane.wtf/0412799a09373f3852b700370dfe795f937b766b44d4eaec71fab85a66f4f766_headshot2.png",
          "version": ""
        }
      ]
    }

## GET /apisite/thumbnails/v1/users/avatar-headshot

Host: octane.wtf

Returns headshot thumbnails.

Response (captured):

    {
      "data": [
        {
          "targetId": 1043,
          "state": "Completed",
          "imageUrl": "https://tcdn.octane.wtf/0412799a09373f3852b700370dfe795f937b766b44d4eaec71fab85a66f4f766_headshot2.png",
          "version": ""
        }
      ]
    }
