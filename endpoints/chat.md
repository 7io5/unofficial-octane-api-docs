# Chat

## GET /v2/metadata

Host: chat.octane.wtf

Returns chat feature flags.

Response (captured):

    {
      "isChatEnabledByPrivacySetting": 1,
      "languageForPrivacySettingUnavailable": "Chat is currently unavailable",
      "maxConversationTitleLength": 150,
      "numberOfMembersForPartyChrome": 6,
      "partyChromeDisplayTimeStampInterval": 300000,
      "signalRDisconnectionResponseInMilliseconds": 3000,
      "typingInChatFromSenderThrottleMs": 5000,
      "typingInChatForReceiverExpirationMs": 8000,
      "relativeValueToRecordUiPerformance": 0,
      "isChatDataFromLocalStorageEnabled": false,
      "chatDataFromLocalStorageExpirationSeconds": 30,
      "isUsingCacheToLoadFriendsInfoEnabled": false,
      "cachedDataFromLocalStorageExpirationMS": 30000,
      "senderTypesForUnknownMessageTypeError": ["User"],
      "isInvalidMessageTypeFallbackEnabled": false,
      "isRespectingMessageTypeEnabled": true,
      "validMessageTypesWhiteList": ["PlainText", "Link"],
      "shouldRespectConversationHasUnreadMessageToMarkAsRead": true,
      "isVoiceChatForClientSideEnabled": false,
      "isAliasChatForClientSideEnabled": true,
      "isPlayTogetherForGameCardsEnabled": true,
      "isRoactChatEnabled": false
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

Response (captured):

    [
      {
        "id": 2525,
        "title": "u10",
        "initiator": {
          "type": "User",
          "targetId": 1114,
          "name": "u10",
          "displayName": "Nuke The Planet"
        },
        "hasUnreadMessages": false,
        "participants": [
          {
            "type": "User",
            "targetId": 1114,
            "name": "u10",
            "displayName": "Nuke The Planet"
          },
          {
            "type": "User",
            "targetId": 1043,
            "name": "Zyko",
            "displayName": "OnlyTwentyCharacters"
          }
        ],
        "conversationType": "OneToOneConversation",
        "conversationTitle": {
          "titleForViewer": "u10",
          "isDefaultTitle": true
        },
        "conversationUniverse": null,
        "lastUpdated": "2026-10-03T20:58:06.901091Z"
      }
    ]

## GET /v2/multi-get-latest-messages

Returns the latest messages for several conversations.

Query params: conversationIds, pageSize.

Response (captured):

    [
      {
        "conversationId": 2525,
        "chatMessages": [
          {
            "id": "6df793f2-dd4a-4830-954a-427baa94ee81",
            "senderType": "User",
            "sent": "2026-10-03T20:58:06.901091Z",
            "read": true,
            "messageType": "PlainText",
            "senderTargetId": 1043,
            "content": "k"
          }
        ]
      }
    ]

## GET /v2/get-messages

Returns messages for a conversation.

Response: not captured.

## POST /v2/send-message

Sends a message.

Response: not captured.

## POST /v2/update-user-typing-status

Updates the typing status of the authenticated user in a conversation.

Response: not captured.
