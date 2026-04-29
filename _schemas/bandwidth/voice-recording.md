---
description: Recording schema from Bandwidth voice API
layout: schema
name: Recording
properties_list:
- description: The unique identifier for the recording
  name: recordingId
  type: string
- description: The Bandwidth account ID
  name: accountId
  type: string
- description: The call ID associated with this recording
  name: callId
  type: string
- description: The application ID
  name: applicationId
  type: string
- description: The duration of the recording in ISO 8601 format
  name: duration
  type: string
- description: The number of audio channels in the recording
  name: channels
  type: integer
- description: The time the recording started
  name: startTime
  type: string
- description: The time the recording ended
  name: endTime
  type: string
- description: The audio format of the recording
  name: fileFormat
  type: string
- description: The status of the recording
  name: status
  type: string
- description: The URL to download the recording media
  name: mediaUrl
  type: string
- description: ''
  name: transcription
  type: object
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-recording-schema.json
slug: voice-recording
source_filename: voice-recording-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-recording-schema.json\",\n  \"title\": \"Recording\",\n  \"description\": \"Recording schema from Bandwidth voice API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recordingId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the recording\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The Bandwidth account ID\"\n    },\n    \"callId\": {\n      \"type\": \"string\",\n      \"description\": \"The call ID associated with this recording\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The application ID\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"The duration of the recording in ISO 8601 format\"\n    },\n    \"channels\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"The number of audio channels in the recording\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the recording started\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the recording ended\"\n    },\n    \"fileFormat\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"wav\",\n        \"mp3\"\n      ],\n      \"description\": \"The audio format of the recording\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"complete\",\n        \"partial\",\n        \"error\"\n      ],\n      \"description\": \"The status of the recording\"\n    },\n    \"mediaUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to download the recording media\"\n    },\n    \"transcription\": {\n      \"$ref\": \"#/components/schemas/Transcription\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-recording-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Recording
---
