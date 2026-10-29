# APIs

## GET /v1/discord/status

Host: apis.octane.wtf

Returns the authenticated user's linked Discord account status.

Response (captured):

    {
      "success": true,
      "data": {
        "linked": true,
        "discordId": "1415706751415750819"
      }
    }

## GET /v1/two-step-verification/status

Host: apis.octane.wtf

Returns the authenticated user's two-step verification status.

Response (captured):

    {
      "enabled": true,
      "staff": false
    }

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
