# Locale

## GET /v1/locales

Returns available locales.

Response (captured):

    {
      "data": [
        {
          "locale": {
            "id": 1,
            "locale": "en_us",
            "name": "English(US)",
            "nativeName": "English",
            "language": {
              "id": 41,
              "name": "English",
              "nativeName": "English",
              "languageCode": "en"
            }
          },
          "isEnabledForFullExperience": true,
          "isEnabledForSignupAndLogin": true,
          "isEnabledForInGameUgc": true
        }
      ]
    }

## GET /v1/locales/user-localization-locus-supported-locales

Returns supported locales for the authenticated user.

Response: not captured.
