# Groups

## GET /v1/groups/{groupId}

Returns group details.

Response (captured):

    {
      "id": 906,
      "name": "OGUsers",
      "description": "Group for the game OGUser's!",
      "memberCount": 29,
      "owner": {
        "id": 1043,
        "name": "bob"
      }
    }

## GET /v1/groups/{groupId}/membership

Returns the authenticated user's membership in a group.

Response (captured):

    {
      "groupId": 906,
      "isPrimary": false,
      "isPendingJoin": false,
      "userRole": {
        "id": 3899,
        "name": "Approved",
        "rank": 1
      },
      "areGroupGamesVisible": true
    }

## GET /v1/groups/{groupId}/roles

Returns group roles.

Response (captured):

    {
      "groupId": 906,
      "roles": [
        {
          "id": 3898,
          "groupId": 906,
          "name": "Guest",
          "description": "A non-group member.",
          "rank": 0,
          "memberCount": 0
        },
        {
          "id": 3899,
          "groupId": 906,
          "name": "Approved",
          "description": "",
          "rank": 1,
          "memberCount": 23
        },
        {
          "id": 4273,
          "groupId": 906,
          "name": "Dev/Admin",
          "description": "",
          "rank": 253,
          "memberCount": 3
        },
        {
          "id": 3900,
          "groupId": 906,
          "name": "Co-owner",
          "description": "",
          "rank": 254,
          "memberCount": 2
        },
        {
          "id": 3901,
          "groupId": 906,
          "name": "Owner",
          "description": "hvs",
          "rank": 255,
          "memberCount": 1
        }
      ]
    }

## GET /v1/groups/metadata

Returns group limits and flags.

Response (captured):

    {
      "groupLimit": 100,
      "currentGroupCount": 2,
      "groupStatusMaxLength": 255,
      "groupPostMaxLength": 500,
      "isGroupWallNotificationsEnabled": false,
      "groupWallNotificationsSubscribeIntervalInMilliseconds": 60000,
      "areProfileGroupsHidden": false,
      "isGroupDetailsPolicyEnabled": true
    }

## GET /v1/groups/{groupId}/roles/{roleId}/users

Returns users in a group role.

Response: not captured.

## GET /v1/groups/{groupId}/social-links

Returns social links for a group.

Response: not captured.

## GET /v1/groups/{groupId}/payouts

Returns group payout info.

Response: not captured.

## GET /v1/groups/search

Searches groups.

Query params: keyword, limit, cursor, sortOrder.

Response: not captured.

## GET /v1/users/{userId}/groups/primary/role

Returns a user's main group role.

Response: not captured.

## GET /v1/users/{userId}/groups/roles

Returns all group roles for a user.

Response: not captured.

## GET /v2/groups/{groupId}/wall/posts

Returns group wall posts.

Response: not captured.
