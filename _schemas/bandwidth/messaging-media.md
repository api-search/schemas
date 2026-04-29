---
description: Media schema from Bandwidth messaging API
layout: schema
name: Media
properties_list:
- description: The name of the media file
  name: mediaName
  type: string
- description: The size of the media file in bytes
  name: contentLength
  type: integer
- description: The MIME type of the media file
  name: contentType
  type: string
- description: The URL to access the media content
  name: content
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/messaging-media-schema.json
slug: messaging-media
source_filename: messaging-media-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/messaging-media-schema.json\",\n  \"title\": \"Media\",\n  \"description\": \"Media schema from Bandwidth messaging API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mediaName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the media file\"\n    },\n    \"contentLength\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the media file in bytes\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the media file\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to access the media content\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/messaging-media-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Media
---
