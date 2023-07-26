---
title: ActivityPub - Delete
---

Used to delete something. It could be a previous request, it could be a user.

Fun fact: when a Mastodon server knows that you exist, you may start getting account deletion requests for accounts
deleted from that server.

## Example

### Request

**POST** to a server's inbox:

```json
{
	"type": "Delete ",
	"@context": "https://www.w3.org/ns/activitystreams ",
	"id": "https://mastodon.social/users/oddevan",
	"actor": "https://mastodon.social/users/oddevan",
	"to": [
		"https://www.w3.org/ns/activitystreams#Public"
	],
	"object": "https://mastodon.social/users/oddevan",
}
```