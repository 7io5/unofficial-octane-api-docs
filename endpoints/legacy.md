# Legacy

These endpoints are maintained for backward compatibility.

## GET /asset/profile-status

Returns the profile status of an asset.

Query params: assetId.

Response: not captured.

## GET /avatar-thumbnail-3d/json

Returns a 3D avatar thumbnail.

Query params: userId.

Response: not captured.

## GET /build/universes

Returns universes for the build page.

Query params: activeOnly, groupId, startRow.

Response: not captured.

## GET /comments/get-json

Returns comments for an asset.

Query params: assetId, startIndex, cachebuster, thumbnailFormat, thumbnailHeight, thumbnailWidth.

Response: not captured.

## GET /game/get-join-script

Returns the join script for a place.

Query params: placeId.

Response: not captured.

## GET /games/getfriendsgameinstances

Returns game instances friends are in.

Query params: placeId.

Response: not captured.

## GET /games/getgameinstancesjson

Returns game instances for a place.

Query params: placeId, startIndex.

Response: not captured.

## GET /games/votingservice/{id}

Returns voting data for a game.

Response: not captured.

## GET /my/settings/json

Returns the authenticated user's settings.

Response: not captured.

## GET /private-server/instance-list-json

Returns private server instances for a universe.

Query params: universeId, page.

Response: not captured.

## GET /recipe?iteration

Returns a recipe.

Response: not captured.

## GET /referral/v1/me

Returns referral info for the authenticated user.

Response: not captured.

## POST /referral/v1/me

Updates referral info for the authenticated user.

Response: not captured.

## GET /search/users/metadata

Returns metadata for the user search.

Response (captured):

    {
      "Keyword": "a",
      "MaxRows": 12,
      "IsPhone": false,
      "IsTablet": false,
      "IsGuest": false,
      "FriendshipStatusValues": [
        "NoFriendship",
        "PendingOnOtherUser",
        "PendingOnCurrentUser",
        "Friends"
      ],
      "CurrentUserId": 1043,
      "InApp": false,
      "InAndroidApp": false,
      "IniOSApp": false,
      "KeywordMinLength": 3,
      "IsChatDisabledByPrivacySetting": false
    }

## GET /search/users/results

Returns user search results.

Query params: keyword, maxRows, startIndex.

Response (captured):

    {
      "Keyword": "a",
      "StartIndex": 0,
      "MaxRows": 5,
      "TotalResults": 0,
      "UserSearchResults": []
    }

## GET /usercheck/show-tos

Checks whether the TOS prompt should be shown.

Response (captured):

    {
      "success": true
    }

## GET /users/favorites/list-json

Returns the authenticated user's favorites.

Query params: assetTypeId, itemsPerPage, userId.

Response: not captured.

## GET /users/inventory/list-json

Returns the authenticated user's inventory.

Query params: assetTypeId, cursor, itemsPerPage, sortOrder, userId.

Response: not captured.

## GET /users/profile/playerassets-json

Returns player assets for a user.

Query params: assetTypeId, userId.

Response: not captured.

## GET /users/profile/robloxcollections-json

Returns roblox collections for a user.

Query params: userId.

Response: not captured.

## POST /abuse-report/v1/report

Submits an abuse report.

Response: not captured.

## POST /authentication/signoutfromallsessionsandreauthenticate

Signs out of all sessions and re-authenticates.

Response: not captured.

## POST /cdn-cgi/rum

Reports real user monitoring metrics.

Response: not captured.

## POST /money.aspx/getmytransactions

Returns the authenticated user's transactions.

Response: not captured.

## POST /promocodes/redeem

Redeems a promo code.

Query params: code.

Response: not captured.

## POST /v1/username

Updates the authenticated user's username.

Response: not captured.
