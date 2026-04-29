---
description: A Threads post.
layout: schema
name: ThreadsMedia
properties_list:
- description: Media ID.
  name: id
  type: string
- description: Media type.
  name: media_type
  type: string
- description: Post text content.
  name: text
  type: string
- description: Permanent URL.
  name: permalink
  type: string
- description: Publishing timestamp.
  name: timestamp
  type: string
- description: Author username.
  name: username
  type: string
- description: Whether this is a quote post.
  name: is_quote_post
  type: boolean
provider_name: Facebook
provider_slug: facebook
schema_file: json-schema/threads-api-threads-media-schema.json
slug: threads-api-threads-media
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/threads-api-threads-media-schema.json\",\n  \"title\": \"ThreadsMedia\",\n  \"description\": \"A Threads post.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Media ID.\" },\n    \"media_type\": { \"type\": \"string\", \"description\": \"Media type.\", \"enum\": [\"TEXT_POST\", \"IMAGE\", \"VIDEO\", \"CAROUSEL_ALBUM\"] },\n    \"text\": { \"type\": \"string\", \"description\": \"Post text content.\" },\n    \"permalink\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"Permanent URL.\" },\n    \"timestamp\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Publishing timestamp.\" },\n    \"username\": { \"type\": \"string\", \"description\": \"Author username.\" },\n    \"is_quote_post\": { \"type\": \"boolean\", \"\
  description\": \"Whether this is a quote post.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/threads-api-threads-media-schema.json
tags:
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
title: ThreadsMedia
---
