# Games

## GET /v1/games

Returns details for multiple universes.

Query params: universeIds.

Response (captured):

    {
      "data": []
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

Response: not captured.

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

Response: not captured.

## GET /v2/groups/{groupId}/games

Returns games made by a group.

Response: not captured.

## GET /v2/games/{universeId}/media

Returns images and videos for a universe.

Response: not captured.
