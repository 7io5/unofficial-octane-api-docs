# Privacy Settings

## GET /v1/privacy

Returns the authenticated user's privacy settings.

Response (captured):

    {
      "isUnder13": false,
      "isPrivacyModeEnabled": false
    }

## GET /v1/privacy/info

Returns privacy info.

Response (captured):

    {
      "isUnder13": false,
      "isPrivacyModeEnabled": false
    }

## GET /v1/inventory-privacy

Returns the authenticated user's inventory privacy setting.

Response (captured):

    {
      "inventoryPrivacy": "AllUsers"
    }

## POST /v1/inventory-privacy

Updates the authenticated user's inventory privacy setting.

Response: not captured.

## GET /v1/trade-privacy

Returns the authenticated user's trade privacy setting.

Response (captured):

    {
      "tradePrivacy": "All"
    }

## POST /v1/trade-privacy

Updates the authenticated user's trade privacy setting.

Response: not captured.

## GET /v1/trade-value

Returns the authenticated user's trade value setting.

Response (captured):

    {
      "tradeValue": "None"
    }

## GET /v1/social/connected-providers

Returns connected social providers.

Response (captured):

    {
      "data": []
    }

## GET /v1/xbox/connection

Returns the authenticated user's Xbox connection status.

Response (captured):

    {
      "isConnected": false,
      "xboxGamertag": null
    }
