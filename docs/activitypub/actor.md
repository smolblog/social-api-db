# Actor

## Request

An empty **GET** request to the server's endpoint for this particular actor.

```
GET /wp-json/smolblog/v2/site/426a9e54-435f-4135-9252-0d0a6ddd1dba/activitypub/actor
```

## Response

## Response Variants

### Smolblog (WIP)

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

### [Micro.blog](../implementations/microblog.md)

```json
{
  "@context": [
    "https://www.w3.org/ns/activitystreams",
    "https://w3id.org/security/v1"
  ],
  "id": "https://micro.blog/activitypub/oddevan",
  "type": "Person",
  "preferredUsername": "oddevan",
  "name": "Evan Hildreth",
  "summary": "Once upon a time, there were two Evans. Even Evan lived across the hall. He was a very proportional man, had good posture, and always kept the salt with the pepper.\n\nI’m odd.",
  "inbox": "https://micro.blog/activitypub/oddevan/inbox",
  "outbox": "https://micro.blog/activitypub/oddevan/outbox",
  "followers": "https://micro.blog/activitypub/oddevan/followers",
  "following": "https://micro.blog/activitypub/oddevan/following",
  "endpoints": { "sharedInbox": "https://micro.blog/activitypub/shared/inbox" },
  "publicKey": {
    "id": "https://micro.blog/activitypub/oddevan#key",
    "owner": "https://micro.blog/activitypub/oddevan",
    "publicKeyPem": "-----BEGIN PUBLIC KEY-----\nMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAo65nMxZaBtDIsl/KtRBR\nWiS/5gIutLil0TlIezKzikVkOe7+8EI3vkQAqKtBULNtJFBlKaqWbSyshLt+sFvU\nLNcugYGWNEFfUdTKC6MSqJCbjE09xRjrOVd6sSYbDwDbJpBhpZpIg1VscHOB3ngi\nO7QHmyf8kbyvy3N1h0lW+6vdqEnmkoJmGDHnhC6ip+Z96G+CXJWIIjT/Bf+dhU20\nmzHE+3+uICr5IQje/rro4pwvedd7FTWHculyvki3uY3iDQswYZA8w0ij13A1khV3\nrjlETVHHDm7J4MtyHyt6mGa9Z1N9zLz9WK7wkRJbLWCKzzQxsPTvEVl+/nCjKHAI\n4QIDAQAB\n-----END PUBLIC KEY-----\n"
  },
  "icon": {
    "url": "https://micro.blog/oddevan/avatar.jpg",
    "type": "Image",
    "mediaType": "image/jpeg"
  },
  "attachment": [
    {
      "type": "PropertyValue",
      "name": "Blog",
      "value": "\u003ca href=\"https://oddevan.com/\"\u003eoddevan.com\u003c/a\u003e"
    }
  ]
}

```