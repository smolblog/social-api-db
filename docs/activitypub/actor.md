---
title: ActivityPub - Actor
---

## Example

### Request

An empty **GET** request to the server's endpoint for this particular actor.

```
GET /wp-json/smolblog/v2/site/426a9e54-435f-4135-9252-0d0a6ddd1dba/activitypub/actor
```

### Response

```json
{
	"type": "Person",
	"streams":[],
	"id": "https:\/\/smol.blog\/wp-json\/smolblog\/v2\/site\/426a9e54-435f-4135-9252-0d0a6ddd1dba\/activitypub\/actor",
	"inbox": "https:\/\/smol.blog\/wp-json\/smolblog\/v2\/site\/426a9e54-435f-4135-9252-0d0a6ddd1dba\/activitypub\/inbox",
	"outbox": "https:\/\/smol.blog\/wp-json\/smolblog\/v2\/site\/426a9e54-435f-4135-9252-0d0a6ddd1dba\/activitypub\/outbox",
	"preferredUsername": "oddevan",
	"url": "http:\/\/oddevan.smol.blog",
	"name": "Evan Hildreth",
	"endpoints": {
		"sharedInbox": "https:\/\/smol.blog\/wp-json\/smolblog\/v2\/activitypub\/inbox"
	},
	"publicKey": {
		"id": "https:\/\/smol.blog\/wp-json\/smolblog\/v2\/site\/426a9e54-435f-4135-9252-0d0a6ddd1dba\/activitypub\/actor#publicKey",
		"owner": "https:\/\/smol.blog\/wp-json\/smolblog\/v2\/site\/426a9e54-435f-4135-9252-0d0a6ddd1dba\/activitypub\/actor",
		"publicKeyPem": "-----BEGIN PUBLIC KEY-----\nMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAyKBsUQR9J+JRQd7pFXO3\nATrJIYcEp309IWapF3Oe\/aEklSenWMZVrLa14jub12WY6SYl981XN4PN0tqTTlSV\naAZDUWDQd1XdGiPHKo37Yo8Qijc7QOu3tWM082ZXC0PKSlfsG\/mLK5bPIY97BUE9\nkk5J93RVTz7mj7Gw\/bnEqB5xiUHxrsqQhblyowuRIj1jVr0iyU0aUzxmEaTDlZ6j\nfsaeEc3FpuvLEJP+fdCTh3gXSg+JvqQ\/fHb+aYbRLqKuuJQ7l7+yxJvLdYuMHkp1\nKBDgoOIeOxoSeFj3i3Bceb2U7QSkolY5RCOo3fTq+GhJXQua2KeL7B5kSefofYyQ\nwQIDAQAB\n-----END PUBLIC KEY-----"
	}
}
```