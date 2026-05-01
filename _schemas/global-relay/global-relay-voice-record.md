---
description: A voice or video call recording archived in the Global Relay Archive, including call metadata, participants, and references to audio/video files.
layout: schema
name: Global Relay Voice Record
properties_list:
- description: Unique identifier for the call or meeting
  name: callId
  type: string
- description: Type of voice/video communication
  name: callType
  type: string
- description: Title or subject of the call or meeting
  name: title
  type: string
- description: Start time of the call in ISO 8601 format
  name: startTime
  type: string
- description: End time of the call in ISO 8601 format
  name: endTime
  type: string
- description: Duration in seconds
  name: duration
  type: integer
- description: List of call participants
  name: participants
  type: array
- description: IDs of audio/video files uploaded via /files endpoint
  name: fileIds
  type: array
- description: Text transcript of the call if available
  name: transcript
  type: string
provider_name: Global Relay
provider_slug: global-relay
schema_file: json-schema/global-relay-voice-record.json
slug: global-relay-voice-record
source_filename: global-relay-voice-record.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"global-relay-voice-record.json\",\n  \"title\": \"Global Relay Voice Record\",\n  \"description\": \"A voice or video call recording archived in the Global Relay Archive, including call metadata, participants, and references to audio/video files.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"callId\",\n    \"callType\",\n    \"startTime\",\n    \"endTime\",\n    \"participants\"\n  ],\n  \"properties\": {\n    \"callId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the call or meeting\"\n    },\n    \"callType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of voice/video communication\",\n      \"enum\": [\n        \"VoiceCall\",\n        \"VideoCall\",\n        \"Conference\",\n        \"Meeting\",\n        \"Webinar\"\n      ]\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title or subject of the call\
  \ or meeting\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of the call in ISO 8601 format\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"End time of the call in ISO 8601 format\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration in seconds\"\n    },\n    \"participants\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"global-relay-participant.json\"\n      },\n      \"description\": \"List of call participants\"\n    },\n    \"fileIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of audio/video files uploaded via /files endpoint\"\n    },\n    \"transcript\": {\n      \"type\": \"string\",\n      \"description\": \"Text transcript of the call if available\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/json-schema/global-relay-voice-record.json
tags:
- Archiving
- Compliance
- Data Retention
- Email Security
- Regulatory Compliance
title: Global Relay Voice Record
---
