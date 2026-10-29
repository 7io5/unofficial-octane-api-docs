# Private Messages

## GET /v1/messages

Host: privatemessages.octane.wtf

Query params: messageTab, pageNumber, pageSize.

Returns the authenticated user's private messages.

Response: not captured.

## POST /v1/messages/send

Host: privatemessages.octane.wtf

Sends a private message.

Response: not captured.

## GET /v1/announcements/metadata

Host: privatemessages.octane.wtf

Returns announcements metadata.

Response: not captured.

## GET /apisite/privatemessages/v1/messages/unread/count

Host: octane.wtf

Returns unread message count.

Response (captured):

    {
      "count": 8
    }

## GET /apisite/privatemessages/v1/messages/{userId}/can-message

Host: octane.wtf

Checks whether the authenticated user can message a target user.

Response: not captured.
