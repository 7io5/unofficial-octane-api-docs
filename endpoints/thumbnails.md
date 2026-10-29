# Thumbnails

## GET /v1/assets

Returns thumbnails for assets.

Query params: assetIds, format, size, returnPolicy.

Response: not captured.

## GET /v1/badges/icons

Returns badge icons.

Response: not captured.

## GET /v1/games/icons

Returns game icons.

Response (captured):

    {
      "data": [
        {
          "targetId": 25070,
          "state": "Completed",
          "imageUrl": "https://tcdn.octane.wtf/66d4eb2385a666a2fca63ecef8910236381b4d53411cfbf057237673d1c6b296.png",
          "version": "TN3"
        }
      ]
    }

## GET /v1/games/multiget/thumbnail

Returns thumbnails for multiple games.

Response: not captured.

## GET /v1/groups/icons

Returns group icons.

Response (captured):

    {
      "data": [
        {
          "targetId": 906,
          "state": "Completed",
          "imageUrl": "https://tcdn.octane.wtf/be4d44d06459f4b901662152a8dbb8409033e80ce5b75e9aca8a6aef53a819db.png",
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
          "targetId": 1224,
          "state": "Completed",
          "imageUrl": "https://tcdn.octane.wtf/5f6bc4d177be4104270bfa338e84dca93260c423d20513569f550461633b1d72_thumbnail.png",
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
          "targetId": 1224,
          "state": "Completed",
          "imageUrl": "https://tcdn.octane.wtf/5f6bc4d177be4104270bfa338e84dca93260c423d20513569f550461633b1d72_headshot2.png",
          "version": ""
        }
      ]
    }
