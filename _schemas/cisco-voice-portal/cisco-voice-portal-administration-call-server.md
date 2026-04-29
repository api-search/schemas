---
description: ''
layout: schema
name: CallServer
properties_list:
- description: ''
  name: serverId
  type: string
- description: ''
  name: hostname
  type: string
- description: ''
  name: ipAddress
  type: string
- description: ''
  name: sipPort
  type: integer
- description: ''
  name: status
  type: string
- description: ''
  name: activeCalls
  type: integer
- description: ''
  name: maxCalls
  type: integer
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-administration-call-server-schema.json
slug: cisco-voice-portal-administration-call-server
source_filename: cisco-voice-portal-administration-call-server-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallServer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serverId\": {\n      \"type\": \"string\"\n    },\n    \"hostname\": {\n      \"type\": \"string\"\n    },\n    \"ipAddress\": {\n      \"type\": \"string\"\n    },\n    \"sipPort\": {\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"activeCalls\": {\n      \"type\": \"integer\"\n    },\n    \"maxCalls\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-administration-call-server-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: CallServer
---
