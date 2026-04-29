---
description: A Facebook post.
layout: schema
name: Post
properties_list:
- description: The post ID.
  name: id
  type: string
- description: Post message text.
  name: message
  type: string
- description: Time the post was created.
  name: created_time
  type: string
- description: Time the post was last updated.
  name: updated_time
  type: string
- description: Post type.
  name: type
  type: string
- description: URL attached to the post.
  name: link
  type: string
- description: Permanent URL to the post.
  name: permalink_url
  type: string
provider_name: Facebook
provider_slug: facebook
schema_file: json-schema/graph-api-post-schema.json
slug: graph-api-post
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/graph-api-post-schema.json\",\n  \"title\": \"Post\",\n  \"description\": \"A Facebook post.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"The post ID.\" },\n    \"message\": { \"type\": \"string\", \"description\": \"Post message text.\" },\n    \"created_time\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Time the post was created.\" },\n    \"updated_time\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Time the post was last updated.\" },\n    \"type\": { \"type\": \"string\", \"description\": \"Post type.\", \"enum\": [\"link\", \"status\", \"photo\", \"video\", \"offer\"] },\n    \"link\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"URL attached to the post.\" },\n    \"permalink_url\"\
  : { \"type\": \"string\", \"format\": \"uri\", \"description\": \"Permanent URL to the post.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/json-schema/graph-api-post-schema.json
tags:
- Advertising
- Content Publishing
- Messaging
- Social Media
- Social Networking
title: Post
---
