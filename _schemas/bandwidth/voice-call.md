---
description: Call schema from Bandwidth voice API
layout: schema
name: Call
properties_list:
- description: The unique identifier for the call
  name: callId
  type: string
- description: The Bandwidth account ID
  name: accountId
  type: string
- description: The application ID associated with the call
  name: applicationId
  type: string
- description: The destination phone number
  name: to
  type: string
- description: The originating phone number
  name: from
  type: string
- description: The direction of the call
  name: direction
  type: string
- description: The current state of the call
  name: state
  type: string
- description: The time the call was initiated
  name: startTime
  type: string
- description: The time the call was answered
  name: answerTime
  type: string
- description: The time the call ended
  name: endTime
  type: string
- description: The reason the call was disconnected
  name: disconnectCause
  type: string
- description: Custom tag attached to the call
  name: tag
  type: string
- description: The URL for this call resource
  name: callUrl
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-call-schema.json
slug: voice-call
source_filename: voice-call-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-call-schema.json\",\n  \"title\": \"Call\",\n  \"description\": \"Call schema from Bandwidth voice API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"callId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the call\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The Bandwidth account ID\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The application ID associated with the call\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"The destination phone number\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"The originating phone number\"\n    },\n    \"direction\": {\n      \"type\": \"string\",\n      \"enum\": [\n   \
  \     \"inbound\",\n        \"outbound\"\n      ],\n      \"description\": \"The direction of the call\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"initiated\",\n        \"answered\",\n        \"completed\"\n      ],\n      \"description\": \"The current state of the call\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the call was initiated\"\n    },\n    \"answerTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the call was answered\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the call ended\"\n    },\n    \"disconnectCause\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the call was disconnected\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Custom tag attached to the\
  \ call\"\n    },\n    \"callUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL for this call resource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-call-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Call
---
