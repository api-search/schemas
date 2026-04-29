---
description: An Instagram media object.
layout: schema
name: InstagramMedia
properties_list:
- description: Media ID.
  name: id
  type: string
- description: Media caption.
  name: caption
  type: string
- description: Media type.
  name: media_type
  type: string
- description: URL to the media.
  name: media_url
  type: string
- description: Permanent URL to the media.
  name: permalink
  type: string
- description: Publishing timestamp.
  name: timestamp
  type: string
- description: Number of likes.
  name: like_count
  type: integer
- description: Number of comments.
  name: comments_count
  type: integer
provider_name: Facebook
provider_slug: facebook
schema_file: json-schema/instagram-api-instagram-media-schema.json
slug: instagram-api-instagram-media
source_filename: instagram-api-instagram-media-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/instagram-api-instagram-media-schema.json\",\n  \"title\": \"InstagramMedia\",\n  \"description\": \"An Instagram media object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Media ID.\" },\n    \"caption\": { \"type\": \"string\", \"description\": \"Media caption.\" },\n    \"media_type\": { \"type\": \"string\", \"description\": \"Media type.\", \"enum\": [\"IMAGE\", \"VIDEO\", \"CAROUSEL_ALBUM\"] },\n    \"media_url\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"URL to the media.\" },\n    \"permalink\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"Permanent URL to the media.\" },\n    \"timestamp\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Publishing timestamp.\" },\n    \"like_count\"\
  : { \"type\": \"integer\", \"description\": \"Number of likes.\" },\n    \"comments_count\": { \"type\": \"integer\", \"description\": \"Number of comments.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/instagram-api-instagram-media-schema.json
tags:
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
title: InstagramMedia
---
