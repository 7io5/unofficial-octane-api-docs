# Groups

## GET /v1/groups/{groupId}

Host: groups.octane.wtf

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

## GET /v1/groups/{groupId}/roles/{roleId}/users

Returns users in a group role.

Query params: cursor, limit, sortOrder.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": [
        {
          "roleId": 2424,
          "buildersClubMembershipType": "None",
          "userId": 1655,
          "username": "o8asob",
          "displayName": "vicoisconfused"
        }
      ]
    }

## GET /v1/groups/{groupId}/social-links

Returns social links for a group.

Response: not captured.

## GET /v1/groups/{groupId}/payouts

Returns group payout info.

Response: not captured.

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

## GET /v1/groups/search

Searches groups.

Query params: keyword, limit, cursor, sortOrder.

Response: not captured.

## GET /v1/users/{userId}/groups/primary/role

Returns a user's main group role.

Response (captured):

    {
      "role": {
        "id": 2426,
        "groupId": 548,
        "name": "Owner",
        "description": "The extension's creator.",
        "rank": 255,
        "memberCount": 1
      },
      "group": {
        "id": 548,
        "name": "Nexus - Octane Extension",
        "description": "nexus is made by zyko. it is open source and free to use. \r\n\r\nlink: https://github.com/zykieboi/nexus",
        "owner": {
          "buildersClubMembershipType": "None",
          "userId": 1043,
          "username": "Zyko",
          "displayName": "OnlyTwentyCharacters"
        },
        "memberCount": 21,
        "isLocked": false,
        "hasVerifiedBadge": false,
        "isBuildersClubOnly": false,
        "publicEntryAllowed": true
      }
    }

## GET /v1/users/{userId}/groups/roles

Returns all group roles for a user.

Response (captured):

    {
      "data": [
        {
          "role": {
            "id": 2426,
            "groupId": 548,
            "name": "Owner",
            "description": "The extension's creator.",
            "rank": 255,
            "memberCount": 1
          },
          "group": {
            "id": 548,
            "name": "Nexus - Octane Extension",
            "description": "nexus is made by zyko. it is open source and free to use.",
            "owner": {
              "buildersClubMembershipType": "None",
              "userId": 1043,
              "username": "Zyko",
              "displayName": "OnlyTwentyCharacters"
            },
            "memberCount": 21,
            "isLocked": false,
            "hasVerifiedBadge": false,
            "isBuildersClubOnly": false,
            "publicEntryAllowed": true
          }
        }
      ]
    }

## GET /v2/groups/{groupId}/wall/posts

Returns group wall posts.

Query params: cursor, limit, sortOrder.

Response (captured):

    {
      "nextPageCursor": null,
      "previousPageCursor": null,
      "data": [
        {
          "id": 2847,
          "poster": {
            "user": {
              "buildersClubMembershipType": "None",
              "userId": 1043,
              "username": "Zyko",
              "displayName": "OnlyTwentyCharacters"
            },
            "role": {
              "id": 0,
              "groupId": 0,
              "name": "Owner",
              "description": "The extension's creator.",
              "rank": 255,
              "memberCount": 1
            }
          },
          "body": "stop acting like nora bro",
          "created": "2026-10-17T08:46:42.528324Z",
          "updated": "2026-10-17T08:46:42.528324Z"
        }
      ]
    }

## POST /v1/groups/{groupId}/wall/posts

Creates a wall post in a group.

Response (captured, 403 when no token):

    {
      "errors": [
        {
          "code": 0,
          "message": "Token Validation Failed"
        }
      ]
    }

## DELETE /v1/groups/{groupId}/wall/posts/{postId}

Deletes a wall post.

Response: not captured.

## GET /apisite/groups/v1/groups/{groupId}

Host: octane.wtf

Returns group details including shout.

Response (captured):

    {
      "id": 548,
      "name": "Nexus - Octane Extension",
      "description": "nexus is made by zyko. it is open source and free to use. \r\n\r\nlink: https://github.com/zykieboi/nexus",
      "memberCount": 21,
      "owner": {
        "buildersClubMembershipType": "None",
        "userId": 1043,
        "username": "Zyko",
        "displayName": "OnlyTwentyCharacters"
      },
      "shout": {
        "poster": {
          "buildersClubMembershipType": "None",
          "userId": 1043,
          "username": "Zyko",
          "displayName": "OnlyTwentyCharacters"
        },
        "body": "Nexus+ is now released for 150 robux and requires a key for access.",
        "created": "2026-10-22T14:43:42.38157Z",
        "updated": "2026-10-22T14:43:42.38157Z"
      },
      "isBuildersClubOnly": false,
      "publicEntryAllowed": true,
      "isLocked": false,
      "hasVerifiedBadge": false
    }
