---
description: Transcription schema from Bandwidth voice API
layout: schema
name: Transcription
properties_list:
- description: The unique identifier for the transcription
  name: id
  type: string
- description: The status of the transcription
  name: status
  type: string
- description: The time the transcription was completed
  name: completedTime
  type: string
- description: The URL of the transcription result
  name: url
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-transcription-schema.json
slug: voice-transcription
source_filename: voice-transcription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-transcription-schema.json\",\n  \"title\": \"Transcription\",\n  \"description\": \"Transcription schema from Bandwidth voice API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the transcription\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"none\",\n        \"available\",\n        \"error\"\n      ],\n      \"description\": \"The status of the transcription\"\n    },\n    \"completedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the transcription was completed\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the transcription result\"\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-transcription-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Transcription
---
