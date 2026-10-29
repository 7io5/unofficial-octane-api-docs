# Asset Game

## POST /game/report-event

Host: assetgame.octane.wtf

Query params: name.

Reports a game event. Requires a valid token.

Response (captured, 403 when no token):

    {
      "errors": [
        {
          "code": 0,
          "message": "Token Validation Failed"
        }
      ]
    }
