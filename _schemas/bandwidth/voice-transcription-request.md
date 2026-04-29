---
description: TranscriptionRequest schema from Bandwidth voice API
layout: schema
name: TranscriptionRequest
properties_list:
- description: The URL to send the transcription completed webhook to
  name: callbackUrl
  type: string
- description: The HTTP method for the transcription webhook
  name: callbackMethod
  type: string
- description: Custom tag for the transcription request
  name: tag
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-transcription-request-schema.json
slug: voice-transcription-request
source_filename: voice-transcription-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-transcription-request-schema.json\",\n  \"title\": \"TranscriptionRequest\",\n  \"description\": \"TranscriptionRequest schema from Bandwidth voice API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"callbackUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to send the transcription completed webhook to\"\n    },\n    \"callbackMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POST\",\n        \"GET\"\n      ],\n      \"default\": \"POST\",\n      \"description\": \"The HTTP method for the transcription webhook\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Custom tag for the transcription request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-transcription-request-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: TranscriptionRequest
---
