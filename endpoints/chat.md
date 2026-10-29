# Chat

## GET /v2/metadata

Returns chat feature flags.

Response (captured):

    {
      "isChatEnabledByPrivacySetting": 1,
      "languageForPrivacySettingUnavailable": "Chat is currently unavailable",
      "maxConversationTitleLength": 150,
      "numberOfMembersForPartyChrome": 6,
      "partyChromeDisplayTimeStampInterval": 300000
    }

## GET /v2/get-unread-conversation-count

Returns how many conversations are unread.

Response (captured):

    {
      "count": 0
    }

## GET /v2/get-user-conversations

Returns the authenticated user's conversations.

Query params: pageNumber, pageSize.

Response: not captured.

## GET /v2/multi-get-latest-messages

Returns the latest messages for several conversations.

Query params: conversationIds, pageSize.

Response: not captured.

## GET /v2/get-messages

Returns messages for a conversation.

Response: not captured.

## POST /v2/send-message

Sends a message.

Response: not captured.

## POST /v2/update-user-typing-status

Updates the typing status of the authenticated user in a conversation.

Response: not captured.
