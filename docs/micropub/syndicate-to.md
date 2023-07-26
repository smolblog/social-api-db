---
title: Micropub - Syndication Config
---

This provides the syndication channels available to the given user. It is often included in the
[config](/micropub/cconfig) endpoint as well.

## Example

### Request

```
GET /micropub?q=syndicate-to HTTP/1.1
Authorization: Bearer 1234567890asdfghjkl
Host: micro.blog
```

### Response

```json
{
  "syndicate-to": [
    { "uid": "medium", "name": "Medium (@oddevan)" },
    { "uid": "linkedin", "name": "LinkedIn (@Evan Hildreth)" },
    { "uid": "mastodon", "name": "Mastodon (@oddevan@mastodon.social)" },
    { "uid": "tumblr", "name": "Tumblr (oddevan.tumblr.com)" },
    { "uid": "flickr", "name": "Flickr (oddEvan)" },
    { "uid": "bluesky", "name": "Bluesky (oddevan.com)" },
    { "uid": "nostr", "name": "Nostr (npub187sqj...)" }
  ]
}
```