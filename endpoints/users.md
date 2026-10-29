# Users

## GET /v1/users/{userId}

Returns user details.

Response (captured):

    {
      "id": 1224,
      "name": "lua",
      "displayName": "lua",
      "description": "&\n<\n>\n\"\n'\n/\n`\n=\n \n\t\n\t\n\\\n:\n(\n)\n;",
      "created": "2026-09-26T11:42:11.615828Z",
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

Response: not captured.

## GET /apisite/users/v1/users/{userId}/username-history

Returns a user's past usernames.

Response: not captured.

## PATCH /v1/users/{userId}/display-names

Updates a user's display name.

Response: not captured.

## POST /v1/users

Creates a new user. Internal use only.

Response: not captured.
