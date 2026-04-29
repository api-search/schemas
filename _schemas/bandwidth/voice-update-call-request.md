---
description: UpdateCallRequest schema from Bandwidth voice API
layout: schema
name: UpdateCallRequest
properties_list:
- description: Set to completed to hang up the call
  name: state
  type: string
- description: The URL to redirect the call to for new BXML instructions
  name: redirectUrl
  type: string
- description: The HTTP method for the redirect webhook
  name: redirectMethod
  type: string
- description: Fallback URL if the primary redirect URL fails
  name: redirectFallbackUrl
  type: string
- description: The HTTP method for the fallback redirect webhook
  name: redirectFallbackMethod
  type: string
- description: A custom string to attach to the call for tracking purposes
  name: tag
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-update-call-request-schema.json
slug: voice-update-call-request
source_filename: voice-update-call-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-update-call-request-schema.json\",\n  \"title\": \"UpdateCallRequest\",\n  \"description\": \"UpdateCallRequest schema from Bandwidth voice API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"completed\"\n      ],\n      \"description\": \"Set to completed to hang up the call\"\n    },\n    \"redirectUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to redirect the call to for new BXML instructions\"\n    },\n    \"redirectMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POST\",\n        \"GET\"\n      ],\n      \"default\": \"POST\",\n      \"description\": \"The HTTP method for the redirect webhook\"\n    },\n    \"redirectFallbackUrl\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Fallback URL if the primary redirect URL fails\"\n    },\n    \"redirectFallbackMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POST\",\n        \"GET\"\n      ],\n      \"default\": \"POST\",\n      \"description\": \"The HTTP method for the fallback redirect webhook\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"description\": \"A custom string to attach to the call for tracking purposes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-update-call-request-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: UpdateCallRequest
---
