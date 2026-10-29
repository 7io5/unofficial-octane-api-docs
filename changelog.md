# Changelog

All notable changes to the Octane API Docs.

## v1.5 — Third Capture

Corrected existing endpoints with real data:

**Account Information**
- Added `isUserBlockEndpointsUpdated` to `/v1/metadata`
- Added `promotionChannelsVisibilityPrivacy` to `/v1/promotion-channels`

**Chat**
- Full `/v2/metadata` feature flags
- Captured `/v2/get-user-conversations` (raw array, not wrapped)
- Captured `/v2/multi-get-latest-messages` (raw array, not wrapped)

**Games**
- Captured `/v1/games`
- Captured `/v1/games/votes`
- Captured `/v2/users/{userId}/games`

**Groups**
- Captured `/v1/groups/{groupId}/roles/{roleId}/users`
- Captured `/v1/users/{userId}/groups/primary/role`
- Captured `/v1/users/{userId}/groups/roles`
- Captured `/v2/groups/{groupId}/wall/posts`

**Locale**
- Captured `/v1/locales/user-localization-locus-supported-locales`

**Notifications**
- Captured `/notifications/negotiate`
- Captured `/notifications/start`

**Trades**
- Captured `/v1/trades/inbound`
- Captured `/v1/trades/outbound`
- Captured `/v1/trades/inactive`
- Captured `/v1/trades/{tradeId}`

**Users**
- Captured `/apisite/users/v1/users/{userId}/status`
- Captured `/apisite/users/v1/users/{userId}/username-history`

**Legacy**
- Captured `/my/settings/json`
- Captured `/comments/get-json`
- Captured `/users/favorites/list-json`
- Captured `/users/profile/playerassets-json`
- Captured `/users/profile/robloxcollections-json`
- Noted `/recipe` returns 404 HTML, not a real API response

Added new endpoints:

**APIs**
- `GET /v1/discord/status`
- `GET /v1/two-step-verification/status`
- `GET /universal-app-configuration/v1/behaviors/account-settings-ui/content`

**Asset Game**
- `POST /game/report-event`

**Captcha**
- `GET /v1/captcha/metadata`

**TCDN**
- `GET /{hash}`
- `GET /asset_{assetId}_{version}_thumbnail3d.json`

**Asset Thumbnail 3D**
- `GET /asset-thumbnail-3d/json`

**Account Settings (host)**
- `GET /v1/app-chat-privacy`

**Realtime**
- `GET /notifications/negotiate`
- `GET /notifications/start`
- `POST /notifications/abort`
- `WS /notifications/connect`

**CDN CGI**
- `POST /cdn-cgi/rum`
- `BEACON /cdn-cgi/rum`

**Referral**
- `GET /referral/v1/me`
- `POST /referral/v1/me`
- `DELETE /referral/v1/me`

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
- Presence responses
- Most catalog search responses
- Badges responses
- Groups search / social-links / payouts
- Games details / place details / playability / favorites / social-links / media
- Chat get-messages / send-message / typing-status responses
- Friends unfriend, get-tags responses
- Home updatestatus response
- Private messages responses
- Referral responses
