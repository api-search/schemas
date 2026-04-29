---
description: UpdateConferenceRequest schema from Bandwidth voice API
layout: schema
name: UpdateConferenceRequest
properties_list:
- description: Set to completed to end the conference and disconnect all members
  name: status
  type: string
- description: URL to redirect the conference to for new BXML instructions
  name: redirectUrl
  type: string
- description: The HTTP method for the redirect webhook
  name: redirectMethod
  type: string
- description: Custom tag for the conference
  name: tag
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-update-conference-request-schema.json
slug: voice-update-conference-request
source_filename: voice-update-conference-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-update-conference-request-schema.json\",\n  \"title\": \"UpdateConferenceRequest\",\n  \"description\": \"UpdateConferenceRequest schema from Bandwidth voice API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"active\",\n        \"completed\"\n      ],\n      \"description\": \"Set to completed to end the conference and disconnect all members\"\n    },\n    \"redirectUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to redirect the conference to for new BXML instructions\"\n    },\n    \"redirectMethod\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POST\",\n        \"GET\"\n      ],\n      \"default\": \"POST\",\n      \"description\": \"The HTTP method for the redirect\
  \ webhook\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Custom tag for the conference\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-update-conference-request-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: UpdateConferenceRequest
---
