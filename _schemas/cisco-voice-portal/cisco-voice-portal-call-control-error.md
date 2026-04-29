---
description: ''
layout: schema
name: Error
properties_list:
- description: ''
  name: code
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: details
  type: string
- description: ''
  name: timestamp
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-call-control-error-schema.json
slug: cisco-voice-portal-call-control-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"details\": {\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-call-control-error-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: Error
---
