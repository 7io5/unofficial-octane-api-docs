# Changelog

All notable changes to the Octane API Docs.

## v1.4 — Notes

- Added disclaimer that docs are not the full API and not official
- Responses marked "not captured" have no confirmed data yet

## v1.3 — Second Capture

16 new endpoints added:

**Chat**
- `GET /v2/get-messages`
- `POST /v2/send-message`
- `POST /v2/update-user-typing-status`

**Friends**
- `POST /v1/users/{userId}/unfriend`

**Contacts**
- `POST /v1/user/get-tags`

**Locale**
- `GET /v1/locales/user-localization-locus-supported-locales`

**Account Settings** (new section)
- `GET /account/settings/account-country`
- `GET /account/settings/account-restrictions`
- `GET /account/settings/app-chat-privacy`
- `GET /account/settings/follow-me-privacy`
- `GET /account/settings/game-chat-privacy`
- `GET /account/settings/private-message-privacy`
- `GET /account/settings/private-server-invite-privacy`

**Home** (new section)
- `POST /home/updatestatus`

**Private Messages** (new host: `privatemessages.octane.wtf`)
- `GET /v1/announcements/metadata`
- `GET /v1/messages`
- `POST /v1/messages/send`

## v1.2 — Item Owners Endpoint

- Added `GET https://inventory.octane.wtf/v2/assets/{assetId}/owners`
- Documented `nextPageCursor`, `owner` (can be null), `serialNumber`, `created`, `updated`

## v1.1 — Real Responses Captured

- Replaced made-up example responses with real captured data
- Fixed `gender` (number), `categories`/`subcategories` (objects), `search/users/results` (PascalCase)
- Noted `games/votes` needs `universeIds` or returns 400
- Marked untested endpoints as "not captured"

## v1.0 — Initial Docs

First version built from the page capture log. Covered account info, avatar, badges, catalog, chat, contacts, economy, friends, games, groups, inventory, locale, metrics, notifications, presence, private messages, premium features, thumbnails, trades, two-step verification, users, themes, privacy settings, and legacy endpoints.

## Still Missing

- Most POST/PATCH/DELETE response bodies
- Trades responses
- Presence responses
- Notifications negotiate/start/abort responses
- Most catalog search responses
- Badges responses
- Groups search / role users / social-links / payouts
- Games details / place details / playability / favorites / social-links / media
- Chat conversations / messages
