# Two-Step Verification

## GET /v1/users/{userId}/configuration

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
