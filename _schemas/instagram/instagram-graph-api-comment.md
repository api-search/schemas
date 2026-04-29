---
description: Comment schema from Instagram Graph API
layout: schema
name: Comment
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: text
  type: string
- description: ''
  name: username
  type: string
- description: ''
  name: timestamp
  type: string
- description: ''
  name: like_count
  type: integer
- description: ''
  name: hidden
  type: boolean
- description: ID of the parent comment if this is a reply.
  name: parent_id
  type: string
provider_name: Instagram
provider_slug: instagram
schema_file: json-schema/instagram-graph-api-comment-schema.json
slug: instagram-graph-api-comment
source_filename: instagram-graph-api-comment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-comment-schema.json\",\n  \"title\": \"Comment\",\n  \"description\": \"Comment schema from Instagram Graph API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"17858893269000001\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"example\": \"Amazing photo!\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"example\": \"fan_account\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T14:30:00+0000\"\n    },\n    \"like_count\": {\n      \"type\": \"integer\",\n      \"example\": 5\n    },\n    \"hidden\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"parent_id\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"ID of the parent comment if this is a reply.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-comment-schema.json
tags:
- Instagram
- Meta
- Photos
- Social Media
- Videos
- Content Publishing
title: Comment
---
