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

Query params: assetId, startIndex, startindex, thumbnailWidth, thumbnailHeight, thumbnailFormat, cachebuster.

Response (captured):

    {
      "IsUserModerator": false,
      "MaxRows": 10,
      "AreCommentsDisabled": false,
      "Comments": []
    }

## POST /comments/post

Posts a comment.

Response (captured, 403 when no token):

    {
      "errors": [
        {
          "code": 0,
          "message": "Token Validation Failed"
        }
      ]
    }

## POST /favorite/toggle

Toggles favorite state for an asset.

Response (captured, 403 when no token):

    {
      "errors": [
        {
          "code": 0,
          "message": "Token Validation Failed"
        }
      ]
    }

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

Response (captured):

    {
      "ChangeUsernameEnabled": true,
      "IsAdmin": false,
      "UserId": 1043,
      "Name": "Zyko",
      "DisplayName": "OnlyTwentyCharacters",
      "IsDisplayNamesEnabled": true,
      "IsEmailOnFile": true,
      "IsEmailVerified": true,
      "IsPhoneFeatureEnabled": true,
      "RobuxRemainingForUsernameChange": 0,
      "PreviousUserNames": "",
      "UseSuperSafePrivacyMode": false,
      "IsSuperSafeModeEnabledForPrivacySetting": false,
      "UseSuperSafeChat": false,
      "IsAppChatSettingEnabled": false,
      "IsGameChatSettingEnabled": false,
      "IsAccountPrivacySettingsV2Enabled": true,
      "IsSetPasswordNotificationEnabled": false,
      "ChangePasswordRequiresTwoStepVerification": false,
      "ChangeEmailRequiresTwoStepVerification": false,
      "UserEmail": "aaa@octane.wtf",
      "UserEmailMasked": true,
      "UserEmailVerified": true,
      "CanHideInventory": true,
      "CanTrade": true,
      "MissingParentEmail": false,
      "IsUpdateEmailSectionShown": true,
      "IsUnder13UpdateEmailMessageSectionShown": false,
      "IsUserConnectedToFacebook": false,
      "IsTwoStepToggleEnabled": false,
      "AgeBracket": 0,
      "UserAbove13": true,
      "ClientIpAddress": "81.229.213.31",
      "AccountAgeInDays": 33,
      "IsOBC": false,
      "IsTBC": false,
      "IsAnyBC": false,
      "IsPremium": false,
      "IsBcRenewalMembership": false,
      "BcExpireDate": "/Date(-0)/",
      "BcRenewalPeriod": null,
      "BcLevel": null,
      "HasCurrencyOperationError": false,
      "CurrencyOperationErrorMessage": null,
      "BlockedUsersModel": {
        "BlockedUserIds": [],
        "BlockedUsers": [],
        "MaxBlockedUsers": 50,
        "Total": 0,
        "Page": 1
      },
      "Tab": null,
      "ChangePassword": false,
      "IsAccountPinEnabled": false,
      "IsAccountRestrictionsFeatureEnabled": false,
      "IsAccountRestrictionsSettingEnabled": false,
      "IsAccountSettingsSocialNetworksV2Enabled": false,
      "IsUiBootstrapModalV2Enabled": true,
      "IsI18nBirthdayPickerInAccountSettingsEnabled": true,
      "InApp": false,
      "MyAccountSecurityModel": {
        "IsEmailSet": true,
        "IsEmailVerified": true,
        "IsTwoStepEnabled": false,
        "ShowSignOutFromAllSessions": true,
        "TwoStepVerificationViewModel": {
          "UserId": 1043,
          "IsEnabled": false,
          "CodeLength": 6,
          "ValidCodeCharacters": null
        }
      },
      "ApiProxyDomain": "https://octane.wtf",
      "AccountSettingsApiDomain": "https://octane.wtf",
      "AuthDomain": "https://octane.wtf",
      "IsDisconnectFbSocialSignOnEnabled": true,
      "IsDisconnectXboxEnabled": true,
      "NotificationSettingsDomain": "https://octane.wtf",
      "AllowedNotificationSourceTypes": [
        "Test",
        "FriendRequestReceived",
        "FriendRequestAccepted",
        "PartyInviteReceived",
        "PartyMemberJoined",
        "ChatNewMessage",
        "PrivateMessageReceived",
        "UserAddedToPrivateServerWhiteList",
        "ConversationUniverseChanged",
        "TeamCreateInvite",
        "GameUpdate",
        "DeveloperMetricsAvailable"
      ],
      "AllowedReceiverDestinationTypes": ["DesktopPush", "NotificationStream"],
      "BlacklistedNotificationSourceTypesForMobilePush": [],
      "MinimumChromeVersionForPushNotifications": 50,
      "PushNotificationsEnabledOnFirefox": true,
      "LocaleApiDomain": "https://octane.wtf",
      "HasValidPasswordSet": true,
      "IsUpdateEmailApiEndpointEnabled": true,
      "FastTrackMember": null,
      "IsFastTrackAccessible": false,
      "HasFreeNameChange": false,
      "IsAgeDownEnabled": false,
      "IsSendVerifyEmailApiEndpointEnabled": true,
      "IsPromotionChannelsEndpointEnabled": true,
      "ReceiveNewsletter": false,
      "SocialNetworksVisibilityPrivacy": 6
    }

## GET /private-server/instance-list-json

Returns private server instances for a universe.

Query params: universeId, page.

Response: not captured.

## GET /recipe

Returns a recipe.

Query params: iteration.

Response (captured): 404 HTML page, not a real API response.

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

Query params: isLicensingTermsCheckNeeded.

Response (captured):

    {
      "success": true
    }

## GET /users/favorites/list-json

Returns the authenticated user's favorites.

Query params: userId, assetTypeId, itemsPerPage.

Response (captured):

    {
      "IsValid": true,
      "Data": {
        "TotalItems": 0,
        "Start": 0,
        "End": 0,
        "Page": 1,
        "ItemsPerPage": 6,
        "PageType": "favorites",
        "Items": []
      }
    }

## GET /users/inventory/list-json

Returns the authenticated user's inventory.

Query params: assetTypeId, cursor, itemsPerPage, sortOrder, userId.

Response: not captured.

## GET /users/profile/playerassets-json

Returns player badges for a user.

Query params: assetTypeId, userId.

Response (captured):

    {
      "Title": "Player Badges",
      "Label": "badges",
      "MaxNumberOfVisibleAssets": 6,
      "UserId": 1043,
      "IsSeeAllHeaderButtonVisible": true,
      "AssetTypeInventoryUrl": "/users/1043/inventory/#!/badges",
      "Assets": [
        {
          "Id": 3292,
          "AssetSeoUrl": "/badges/3292/Survived-50-Disasters",
          "Thumbnail": {
            "Final": true,
            "Url": "/thumbs/asset.ashx?assetId=3292&width=420&height=420&format=png",
            "RetryUrl": null,
            "UserId": 0,
            "EndpointType": "Avatar"
          },
          "Name": "Survived 50 Disasters",
          "FormatName": null,
          "Description": null,
          "AssetRestrictionIcon": null,
          "HasPremiumBenefit": false
        }
      ]
    }

## GET /users/profile/robloxcollections-json

Returns roblox collections for a user.

Query params: userId.

Response (captured):

    {
      "CollectionsItems": [
        {
          "Id": 20056,
          "AssetSeoUrl": "/catalog/20056/Chill-Classic",
          "Name": "Chill Classic",
          "FormatName": null,
          "Thumbnail": {
            "Final": true,
            "Url": "/thumbs/asset.ashx?assetId=20056&width=420&height=420&format=png",
            "Id": 20056
          },
          "AssetRestrictionIcon": {
            "TooltipText": null,
            "CssTag": "limited",
            "LoadAssetRestrictionIconCss": false,
            "HasTooltip": false
          }
        }
      ]
    }

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

Response (captured, 403 when no token):

    {
      "errors": [
        {
          "code": 0,
          "message": "Token Validation Failed"
        }
      ]
    }

## POST /v1/username

Updates the authenticated user's username.

Response: not captured.
