---
description: Media schema from Instagram Graph API
layout: schema
name: Media
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: caption
  type: string
- description: ''
  name: media_type
  type: string
- description: ''
  name: media_url
  type: string
- description: Thumbnail URL for videos.
  name: thumbnail_url
  type: string
- description: ''
  name: permalink
  type: string
- description: ''
  name: shortcode
  type: string
- description: ''
  name: timestamp
  type: string
- description: ''
  name: like_count
  type: integer
- description: ''
  name: comments_count
  type: integer
- description: ''
  name: is_comment_enabled
  type: boolean
- description: ''
  name: is_shared_to_feed
  type: boolean
- description: Alt text for accessibility.
  name: alt_text
  type: string
- description: ''
  name: username
  type: string
provider_name: Instagram
provider_slug: instagram
schema_file: json-schema/instagram-graph-api-media-schema.json
slug: instagram-graph-api-media
source_filename: instagram-graph-api-media-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-media-schema.json\",\n  \"title\": \"Media\",\n  \"description\": \"Media schema from Instagram Graph API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"17854360229135492\"\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"example\": \"Beautiful sunset at the beach! #photography\"\n    },\n    \"media_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IMAGE\",\n        \"VIDEO\",\n        \"CAROUSEL_ALBUM\",\n        \"REELS\",\n        \"STORIES\"\n      ],\n      \"example\": \"IMAGE\"\n    },\n    \"media_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://scontent.cdninstagram.com/media/example.jpg\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Thumbnail URL for videos.\"\n    },\n    \"permalink\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.instagram.com/p/ABC123/\"\n    },\n    \"shortcode\": {\n      \"type\": \"string\",\n      \"example\": \"ABC123\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00+0000\"\n    },\n    \"like_count\": {\n      \"type\": \"integer\",\n      \"example\": 250\n    },\n    \"comments_count\": {\n      \"type\": \"integer\",\n      \"example\": 15\n    },\n    \"is_comment_enabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"is_shared_to_feed\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"alt_text\": {\n      \"type\": \"string\",\n      \"description\": \"Alt text for accessibility.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"example\": \"examplebusiness\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-media-schema.json
tags:
- Instagram
- Meta
- Photos
- Social Media
- Videos
- Content Publishing
title: Media
---
