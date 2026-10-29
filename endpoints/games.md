# Games

## GET /v1/games

Host: games.octane.wtf

Returns details for multiple universes.

Query params: universeIds.

Response (captured):

    {
      "data": [
        {
          "id": 29626,
          "rootPlaceId": 409001,
          "name": "Zyko's Place Number 4",
          "description": null,
          "sourceName": "Zyko's Place Number 4",
          "sourceDescription": "",
          "creator": {
            "id": 1043,
            "name": "Zyko",
            "type": "User",
            "isRNVAccount": false,
            "hasVerifiedBadge": false
          },
          "price": null,
          "allowedGearGenres": ["All"],
          "allowedGearCategories": [],
          "isGenreEnforced": true,
          "copyingAllowed": false,
          "playing": 0,
          "visits": 0,
          "maxPlayers": 10,
          "created": "2026-10-28T17:11:37.171443Z",
          "updated": "2026-10-28T17:11:37.171443Z",
          "studioAccessToApisAllowed": false,
          "createVipServersAllowed": false,
          "privateServerPrice": null,
          "universeAvatarType": "PlayerChoice",
          "genre": "All",
          "isAllGenre": true,
          "isFavoritedByUser": false,
          "favoritedCount": 0
        }
      ]
    }

## GET /v1/games/list

Returns a list of games.

Response (captured):

    {
      "games": ["..."]
    }

## GET /v1/games/sorts

Returns game sort categories.

Response (captured):

    {
      "sorts": ["..."]
    }

## GET /v1/games/votes

Returns vote data for multiple universes.

Query params: universeIds. Required, otherwise returns 400.

Response (captured):

    {
      "data": [
        {
          "id": 29626,
          "upVotes": 0,
          "downVotes": 0
        }
      ]
    }

## GET /v1/games/multiget-place-details

Returns place details for multiple place IDs.

Query params: placeIds.

Response: not captured.

## GET /v1/games/multiget-playability-status

Returns playability status for multiple universes.

Query params: universeIds.

Response: not captured.

## GET /v1/games/{universeId}/favorites

Returns favorite count for a universe.

Response: not captured.

## GET /v1/games/{universeId}/social-links/list

Returns social links for a universe.

Response: not captured.

## GET /v2/users/{userId}/games

Returns games made by a user.

Query params: limit.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": [
        {
          "id": 29626,
          "name": "Zyko's Place Number 4",
          "description": null,
          "rootPlace": {
            "id": 409001,
            "type": "Place"
          },
          "created": "2026-10-28T17:11:37.171443Z",
          "updated": "2026-10-28T17:11:37.171443Z",
          "placeVisits": 0
        }
      ]
    }

## GET /v2/groups/{groupId}/games

Returns games made by a group.

Response: not captured.

## GET /v2/games/{universeId}/media

Returns images and videos for a universe.

Response: not captured.
