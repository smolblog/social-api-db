# Actor

## Request

An empty **GET** request to the server's endpoint for this particular actor.

```
GET /wp-json/smolblog/v2/site/426a9e54-435f-4135-9252-0d0a6ddd1dba/activitypub/actor
```

## Response

## Response Variants

### [Mastodon](../implementations/mastodon.md)

The **GET** request must be sent with a header of `Accept: application/json` in order to get the response; any other
header will redirect to the HTML profile of the user.

```json
{
  "@context": [
    "https://www.w3.org/ns/activitystreams",
    "https://w3id.org/security/v1",
    {
      "manuallyApprovesFollowers": "as:manuallyApprovesFollowers",
      "toot": "http://joinmastodon.org/ns#",
      "featured": { "@id": "toot:featured", "@type": "@id" },
      "featuredTags": { "@id": "toot:featuredTags", "@type": "@id" },
      "alsoKnownAs": { "@id": "as:alsoKnownAs", "@type": "@id" },
      "movedTo": { "@id": "as:movedTo", "@type": "@id" },
      "schema": "http://schema.org#",
      "PropertyValue": "schema:PropertyValue",
      "value": "schema:value",
      "discoverable": "toot:discoverable",
      "Device": "toot:Device",
      "Ed25519Signature": "toot:Ed25519Signature",
      "Ed25519Key": "toot:Ed25519Key",
      "Curve25519Key": "toot:Curve25519Key",
      "EncryptedMessage": "toot:EncryptedMessage",
      "publicKeyBase64": "toot:publicKeyBase64",
      "deviceId": "toot:deviceId",
      "claim": { "@type": "@id", "@id": "toot:claim" },
      "fingerprintKey": { "@type": "@id", "@id": "toot:fingerprintKey" },
      "identityKey": { "@type": "@id", "@id": "toot:identityKey" },
      "devices": { "@type": "@id", "@id": "toot:devices" },
      "messageFranking": "toot:messageFranking",
      "messageType": "toot:messageType",
      "cipherText": "toot:cipherText",
      "suspended": "toot:suspended",
      "focalPoint": { "@container": "@list", "@id": "toot:focalPoint" }
    }
  ],
  "id": "https://mastodon.social/users/oddevan",
  "type": "Person",
  "following": "https://mastodon.social/users/oddevan/following",
  "followers": "https://mastodon.social/users/oddevan/followers",
  "inbox": "https://mastodon.social/users/oddevan/inbox",
  "outbox": "https://mastodon.social/users/oddevan/outbox",
  "featured": "https://mastodon.social/users/oddevan/collections/featured",
  "featuredTags": "https://mastodon.social/users/oddevan/collections/tags",
  "preferredUsername": "oddevan",
  "name": "Evan Hildreth",
  "summary": "\u003cp\u003eHow long should it take somebody\u2028 / Before he can be someone?\u003c/p\u003e",
  "url": "https://mastodon.social/@oddevan",
  "manuallyApprovesFollowers": false,
  "discoverable": true,
  "published": "2017-11-13T00:00:00Z",
  "devices": "https://mastodon.social/users/oddevan/collections/devices",
  "publicKey": {
    "id": "https://mastodon.social/users/oddevan#main-key",
    "owner": "https://mastodon.social/users/oddevan",
    "publicKeyPem": "-----BEGIN PUBLIC KEY-----\nMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAoDim3Qywy7PQv6YmBxfO\nDCJAasbmCowLQznpaLubJbWCHePer05HMeFYTarPML8lJ+gYoMg9trUzFHBdKbga\nOODwMQyFhN1gjuOnVmF9e92lZhtq+L+6D9Uyg2yzzkqgbfKP0tLchUx/nAC0PA3T\nMTM2pvz3HQH7KTZ37QHTCzEfJcbSRP4YfXUxQiGuDGADGjgRQXzOfYh76uDYpGrn\nGnrjhZvE0S9i1c/7co+1U0GUjeF3o707TfjoGHCeocHtNrOPvNorCrWHjwQJbLaz\nmSDnVvGTsQ/W2jM8i6bMgkdH9UYuCVR8gmIJfpFP70aDbH3NrdLLJpi2AMCggsCx\nhQIDAQAB\n-----END PUBLIC KEY-----\n"
  },
  "tag": [],
  "attachment": [
    { "type": "PropertyValue", "name": "Pronouns", "value": "He/him/his" },
    {
      "type": "PropertyValue",
      "name": "Cross-posted from",
      "value": "\u003cspan class=\"h-card\" translate=\"no\"\u003e\u003ca href=\"https://micro.blog/activitypub/oddevan\" class=\"u-url mention\"\u003e@\u003cspan\u003eoddevan@micro.blog\u003c/span\u003e\u003c/a\u003e\u003c/span\u003e"
    },
    {
      "type": "PropertyValue",
      "name": "Website",
      "value": "\u003ca href=\"https://eph.me/\" target=\"_blank\" rel=\"nofollow noopener noreferrer me\" translate=\"no\"\u003e\u003cspan class=\"invisible\"\u003ehttps://\u003c/span\u003e\u003cspan class=\"\"\u003eeph.me/\u003c/span\u003e\u003cspan class=\"invisible\"\u003e\u003c/span\u003e\u003c/a\u003e"
    }
  ],
  "endpoints": { "sharedInbox": "https://mastodon.social/inbox" },
  "icon": {
    "type": "Image",
    "mediaType": "image/png",
    "url": "https://files.mastodon.social/accounts/avatars/000/238/202/original/b067f50fd338a482.png"
  },
  "image": {
    "type": "Image",
    "mediaType": "image/jpeg",
    "url": "https://files.mastodon.social/accounts/headers/000/238/202/original/e93ad6bcc8ef808a.jpg"
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