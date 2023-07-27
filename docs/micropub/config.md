---
title: Config
---

# Config

This informs the Micropub client what capabilities the server has for the authenticated user.

## Request

```http
GET /micropub?q=config HTTP/1.1
Authorization: Bearer 1234567890asdfghjkl
Host: micro.blog
```

## Response

```json
{
  "media-endpoint": "https://micro.blog/micropub/media",
  "destination": [
    {
      "uid": "https://oddevan.micro.blog/",
      "name": "oddevan.com",
      "microblog-audio": false,
      "microblog-default": false,
      "microblog-title": "Evan Hildreth"
    },
    {
      "uid": "https://oddevan-test.micro.blog/",
      "name": "oddevan-test.micro.blog",
      "microblog-audio": false,
      "microblog-default": false,
      "microblog-title": "Evan Hildreth"
    }
  ],
  "post-types": [
    {
      "type": "note",
      "name": "Post",
      "properties": [
        "content",
        "published",
        "post-status",
        "category",
        "read-of",
        "mp-destination",
        "checkin",
        "location"
      ]
    },
    {
      "type": "article",
      "name": "Article",
      "properties": [
        "name",
        "content",
        "published",
        "post-status",
        "category",
        "mp-channel",
        "mp-destination"
      ]
    },
    {
      "type": "photo",
      "name": "Photo",
      "properties": [
        "name",
        "content",
        "published",
        "post-status",
        "category",
        "mp-destination",
        "photo",
        "mp-photo-alt"
      ]
    },
    {
      "type": "reply",
      "name": "Reply",
      "properties": ["content", "in-reply-to"]
    },
    { "type": "bookmark", "name": "Bookmark", "properties": ["bookmark-of"] }
  ],
  "channels": [
    { "uid": "default", "name": "Posts" },
    { "uid": "pages", "name": "Pages" }
  ],
  "syndicate-to": [
    { "uid": "tumblr", "name": "Tumblr (isthatwhy-everything-is-on-fire.tumblr.com)" },
    { "uid": "bluesky", "name": "Bluesky (oddevan.com)" },
  ]
}
```