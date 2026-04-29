---
description: Media schema from X API v2
layout: schema
name: Media
properties_list:
- description: The height of the media in pixels.
  name: height
  type: integer
- description: The Media Key identifier for this attachment.
  name: media_key
  type: string
- description: ''
  name: type
  type: string
- description: The width of the media in pixels.
  name: width
  type: integer
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-media-schema.json
slug: x-api-media
source_filename: x-api-media-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-media-schema.json\",\n  \"title\": \"Media\",\n  \"description\": \"Media schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"The height of the media in pixels.\",\n      \"minimum\": 0\n    },\n    \"media_key\": {\n      \"type\": \"string\",\n      \"description\": \"The Media Key identifier for this attachment.\",\n      \"pattern\": \"^([0-9]+)_([0-9]+)$\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"The width of the media in pixels.\",\n      \"minimum\": 0\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-media-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: Media
---
