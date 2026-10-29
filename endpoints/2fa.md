# Two-Step Verification

## GET /v1/users/{userId}/configuration

Host: twostepverification.octane.wtf

Returns two-step verification configuration for a user.

Response (captured):

    {
      "primaryMediaType": "Email",
      "methods": [
        {
          "mediaType": "Email",
          "enabled": true
        }
      ]
    }

## GET /v1/two-step-verification/status

Host: apis.octane.wtf

Returns two-step verification status for the authenticated user.

Response (captured):

    {
      "enabled": true,
      "staff": false
    }
