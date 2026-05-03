---
description: A streaming platform supported by Restream for multistreaming destinations.
layout: schema
name: Platform
properties_list:
- description: Unique platform identifier
  name: id
  type: integer
- description: Platform name (e.g., Twitch, YouTube, Facebook)
  name: name
  type: string
- description: Platform website URL
  name: url
  type: string
- description: Platform logo images
  name: image
  type: object
provider_name: Restream
provider_slug: restream
schema_file: json-schema/restream-platform-schema.json
slug: restream-platform
source_filename: restream-platform-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.restream.io/schemas/platform\",\n  \"title\": \"Platform\",\n  \"description\": \"A streaming platform supported by Restream for multistreaming destinations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique platform identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Platform name (e.g., Twitch, YouTube, Facebook)\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Platform website URL\"\n    },\n    \"image\": {\n      \"type\": \"object\",\n      \"description\": \"Platform logo images\",\n      \"properties\": {\n        \"png\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"PNG image URL\"\n        },\n        \"svg\": {\n          \"type\": \"string\",\n\
  \          \"format\": \"uri\",\n          \"description\": \"SVG image URL\"\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restream/refs/heads/main/json-schema/restream-platform-schema.json
tags:
- Broadcast
- Chat
- Content Delivery
- Live Streaming
- Multistreaming
- Video Streaming
title: Platform
---
