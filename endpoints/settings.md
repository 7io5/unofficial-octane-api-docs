# Account Settings

## GET /universal-app-configuration/v1/behaviors/account-settings-ui/content

Host: apis.octane.wtf

Returns which account settings sections are displayed.

Response (captured):

    {
      "displayTwoStepVerification": true,
      "displayAccountPIN": true,
      "displayEmailAddress": true,
      "displayWeChat": false,
      "displayQQ": false,
      "displayConnectedAccounts": true,
      "displayNotificationStream": true,
      "displayDesktopPush": true,
      "displayMobilePush": true,
      "displayPhoneNumber": true,
      "displaySocialMedia": true,
      "displayDescription": true,
      "displayAccountRestrictions": true,
      "displayCountryList": true,
      "displayWhoCanMessageMe": true,
      "displayWhoCanFindMeByPhoneNumber": true,
      "displayWhoCanInviteMeToVIPServers": false,
      "displayWhoCanTradeWithMe": true,
      "displayTradeQualityFilter": true,
      "displayLanguageList": true,
      "displayChangeUsername": true,
      "displayChangePassword": true,
      "displayBillingTab": true,
      "displayPrivacyModeToolTip": true,
      "displayIdentityVerification": true,
      "displayVoiceChatSettings": true,
      "displayPasswordRow": true
    }

## GET /account/settings/account-country

Host: octane.wtf

Returns the authenticated user's account country.

Response (captured):

    {
      "countryCode": "US",
      "countryName": "United States"
    }

## GET /account/settings/account-restrictions

Host: octane.wtf

Returns the authenticated user's account restrictions.

Response (captured):

    {
      "isAccountRestrictionsEnabled": false
    }

## GET /account/settings/app-chat-privacy

Host: octane.wtf

Returns the authenticated user's app chat privacy setting.

Response (captured):

    {
      "appChatPrivacy": "AllUsers"
    }

## GET /account/settings/countries

Host: octane.wtf

Returns the list of selectable countries.

Response (captured):

    []

## GET /account/settings/follow-me-privacy

Host: octane.wtf

Returns the authenticated user's follow-me privacy setting.

Response (captured):

    {
      "FollowMePrivacy": "All"
    }

## GET /account/settings/game-chat-privacy

Host: octane.wtf

Returns the authenticated user's game chat privacy setting.

Response (captured):

    {
      "gameChatPrivacy": "AllUsers"
    }

## GET /account/settings/private-message-privacy

Host: octane.wtf

Returns the authenticated user's private message privacy setting.

Response (captured):

    {
      "PrivateMessagePrivacy": "All"
    }

## GET /account/settings/private-server-invite-privacy

Host: octane.wtf

Returns the authenticated user's private server invite privacy setting.

Response (captured):

    {
      "privateServerInvitePrivacy": "AllUsers"
    }

## GET /account/settings/settings-groups

Host: octane.wtf

Returns the account settings groups.

Response (captured):

    [
      {
        "suffix": "info",
        "title": "Account Info"
      },
      {
        "suffix": "security",
        "title": "Security"
      },
      {
        "suffix": "privacy",
        "title": "Privacy"
      },
      {
        "suffix": "referrals",
        "title": "Referrals"
      }
    ]

## GET /admin-api/api/permissions

Host: octane.wtf

Returns the authenticated user's admin permissions.

Response (captured):

    {
      "rank": {
        "name": null,
        "details": {
          "isAdmin": false,
          "isModerator": false,
          "isOwner": false,
          "canResetTwoStep": false,
          "canIpBan": false
        },
        "permissions": []
      }
    }
