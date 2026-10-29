# Friends

## GET /v1/users/{userId}/friends

Host: friends.octane.wtf

Returns a user's friends list.

Response (captured):

    {
      "data": [
        {
          "isOnline": false,
          "isDeleted": false,
          "isBanned": false,
          "id": 77,
          "name": "chris",
          "displayName": "chris",
          "description": null,
          "presence": {
            "userPresenceType": 1,
            "lastLocation": "Website",
            "rootPlaceId": 0
          },
          "created": "0001-01-01T00:00:00",
          "presenceType": 0,
          "externalAppDisplayName": null,
          "friendFrequentRank": 1,
          "friendFrequentScore": 0
        }
      ]
    }

## GET /v1/users/{userId}/friends/statuses

Query params: userIds.

Returns online statuses for a list of friends.

Response (captured):

    {
      "data": [
        {
          "id": 2020,
          "status": "NotFriends"
        }
      ]
    }

## POST /v1/users/{userId}/unfriend

Removes a user from the authenticated user's friends list.

Response: not captured.

## GET /v1/metadata

Host: friends.octane.wtf

Query params: targetUserId.

Returns friend metadata for a user.

Response (captured):

    {
      "isNearbyUpsellEnabled": false,
      "isFriendsUserDataStoreCacheEnabled": false,
      "userName": "Zyko",
      "displayName": "OnlyTwentyCharacters"
    }

## GET /v1/my/friends/requests

Host: friends.octane.wtf

Query params: limit.

Returns pending friend requests.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": [
        {
          "isOnline": false,
          "isDeleted": false,
          "isBanned": false,
          "id": 22546,
          "name": "44472837",
          "displayName": "Illumination Compero",
          "description": null,
          "presence": null,
          "created": "0001-01-01T00:00:00",
          "presenceType": 0,
          "externalAppDisplayName": null,
          "friendFrequentRank": 1,
          "friendFrequentScore": 0
        }
      ]
    }

## POST /v1/user/friend-requests/decline-all

Host: friends.octane.wtf

Declines all pending friend requests.

Response: not captured (returned 404 in capture).

## POST /v1/users/{userId}/accept-friend-request

Host: friends.octane.wtf

Accepts a friend request from a user.

Response (captured, 403 when no token):

    {
      "errors": [
        {
          "code": 0,
          "message": "Token Validation Failed"
        }
      ]
    }

## GET /v1/users/{userId}/followers

Host: friends.octane.wtf

Query params: sortOrder, limit.

Returns a user's followers.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": [
        {
          "isOnline": false,
          "isDeleted": false,
          "isBanned": false,
          "id": 20620,
          "name": "Tomato_lover",
          "displayName": "Tomato_lover",
          "description": null,
          "presence": null,
          "created": "0001-01-01T00:00:00",
          "presenceType": 0,
          "externalAppDisplayName": null,
          "friendFrequentRank": 1,
          "friendFrequentScore": 0
        }
      ]
    }

## GET /v1/users/{userId}/followings

Host: friends.octane.wtf

Query params: sortOrder, limit.

Returns who a user follows.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": []
    }

## GET /v1/user/friend-requests/count

Host: friends.octane.wtf

Returns pending friend request count.

Response (captured):

    {
      "count": 1
    }

## GET /v1/users/{userId}/followers/count

Host: friends.octane.wtf

Returns follower count.

Response (captured):

    {
      "count": 2
    }

## GET /v1/users/{userId}/followings/count

Host: friends.octane.wtf

Returns following count.

Response (captured):

    {
      "count": 0
    }

## POST /apisite/friends/v1/user/following-exists

Host: octane.wtf

Checks whether a following relationship exists.

Response (captured, 403 when no token):

    {
      "errors": [
        {
          "code": 0,
          "message": "Token Validation Failed"
        }
      ]
    }

## GET /apisite/friends/v1/user/friend-requests/count

Host: octane.wtf

Returns pending friend request count.

Response (captured):

    {
      "count": 1
    }

## GET /apisite/friends/v1/users/{userId}/followers/count

Host: octane.wtf

Returns follower count.

Response (captured):

    {
      "count": 2
    }

## GET /apisite/friends/v1/users/{userId}/followings/count

Host: octane.wtf

Returns following count.

Response (captured):

    {
      "count": 0
    }

## GET /apisite/friends/v1/users/{userId}/friends

Host: octane.wtf

Returns a user's friends list.

Response (captured): same shape as /v1/users/{userId}/friends.

## GET /apisite/friends/v1/users/{userId}/friends/statuses

Host: octane.wtf

Query params: userIds.

Returns online statuses for a list of friends.

Response (captured):

    {
      "data": [
        {
          "id": 1043,
          "status": "NotFriends"
        }
      ]
    }
