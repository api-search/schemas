---
description: ''
layout: schema
name: DeviceCreateRequest
properties_list:
- description: ''
  name: hostname
  type: string
- description: ''
  name: ipAddress
  type: string
- description: ''
  name: deviceType
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: credentials
  type: object
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-administration-device-create-request-schema.json
slug: cisco-voice-portal-administration-device-create-request
source_filename: cisco-voice-portal-administration-device-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeviceCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hostname\": {\n      \"type\": \"string\"\n    },\n    \"ipAddress\": {\n      \"type\": \"string\"\n    },\n    \"deviceType\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"credentials\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-administration-device-create-request-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: DeviceCreateRequest
---
