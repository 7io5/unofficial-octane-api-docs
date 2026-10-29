# Themes

## GET /v1/themes/types

Host: octane.wtf

Returns available theme types.

Response (captured):

    {
      "data": ["Light", "Dark"]
    }

## GET /v1/themes/user

Returns the authenticated user's theme settings.

Response (captured):

    {
      "themeType": "Light",
      "halloweenTheme": false,
      "classicCreatePage": true
    }

## GET /apisite/accountsettings/v1/themes/user

Host: octane.wtf

Returns the authenticated user's theme settings.

Response (captured):

    {
      "themeType": "Light",
      "halloweenTheme": false,
      "classicCreatePage": true
    }

## PATCH /v1/themes/user

Updates the authenticated user's theme settings.

Response: not captured.
