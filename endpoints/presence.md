# Presence

## POST /v1/presence/users

Host: presence.octane.wtf

Returns presence data for multiple users.

Response (captured, 403 when no token):

    {
      "errors": [
        {
          "code": 0,
          "message": "Token Validation Failed"
        }
      ]
    }

## POST /v1/presence/register-app-presence

Host: presence.octane.wtf

Registers app presence for the authenticated user.

Response: not captured.

## POST /apisite/presence/v1/presence/users

Host: octane.wtf

Returns presence data for multiple users.

Response (captured, 403 when no token):

    {
      "errors": [
        {
          "code": 0,
          "message": "Token Validation Failed"
        }
      ]
    }
