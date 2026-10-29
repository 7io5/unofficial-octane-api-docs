# Friends

## GET /v1/users/{userId}/friends

Returns a user's friends list.

Response (captured):

    {
      "data": [
        {
          "id": 1,
          "name": "Octane",
          "displayName": "Octane",
          "isOnline": false
        }
      ]
    }

## GET /v1/users/{userId}/friends/statuses

Returns online statuses for a list of friends.

Query params: userIds.

Response: not captured.

## POST /v1/users/{userId}/unfriend

Removes a user from the authenticated user's friends list.

Response: not captured.

## GET /apisite/friends/v1/users/{userId}/followers/count

Returns follower count.

Response: not captured.

## GET /apisite/friends/v1/users/{userId}/followings/count

Returns following count.

Response: not captured.

## GET /apisite/friends/v1/user/friend-requests/count

Returns pending friend request count.

Response: not captured.

## POST /apisite/friends/v1/user/following-exists

Checks whether a following relationship exists.

Response: not captured.
