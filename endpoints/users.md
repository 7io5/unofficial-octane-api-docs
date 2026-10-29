# Users

## GET /v1/users/{userId}

Host: users.octane.wtf

Returns user details.

Response (captured):

    {
      "id": 1043,
      "name": "Zyko",
      "displayName": "OnlyTwentyCharacters",
      "description": "check out my extension for octane 👀\nhttps://github.com/zykieboi/nexus",
      "created": "2026-09-26T09:27:12.303565Z",
      "isBanned": false,
      "hasVerifiedBadge": false,
      "isPremium": false,
      "hasAdminBadge": false
    }

## GET /apisite/users/v1/users/{userId}

Host: octane.wtf

Returns user details.

Response (captured):

    {
      "id": 1043,
      "name": "Zyko",
      "displayName": "OnlyTwentyCharacters",
      "description": "check out my extension for octane 👀\nhttps://github.com/zykieboi/nexus",
      "created": "2026-09-26T09:27:12.303565Z",
      "isBanned": false,
      "hasVerifiedBadge": false,
      "isPremium": false,
      "hasAdminBadge": false
    }

## GET /apisite/users/v1/users/authenticated

Returns the authenticated user.

Response: same shape as /v1/users/{userId}.

## GET /apisite/users/v1/users/{userId}/status

Returns a user's status.

Response (captured):

    {
      "status": "hello octane my name is zyk and im testing api"
    }

## GET /apisite/users/v1/users/{userId}/username-history

Query params: limit, cursor.

Returns a user's past usernames.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": []
    }

## PATCH /v1/users/{userId}/display-names

Updates a user's display name.

Response: not captured.

## POST /v1/users

Creates a new user. Internal use only.

Response: not captured.

## GET /apisite/accountinformation/v1/users/{userId}/roblox-badges

Host: octane.wtf

Returns roblox badges for a user.

Response (captured):

    []

## GET /apisite/api/alerts/alert-info

Host: octane.wtf

Returns alert info.

Response (captured):

    {
      "IsVisible": false,
      "Text": "",
      "LinkText": "",
      "LinkUrl": ""
    }
