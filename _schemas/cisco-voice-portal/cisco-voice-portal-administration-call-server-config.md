---
description: ''
layout: schema
name: CallServerConfig
properties_list:
- description: ''
  name: serverId
  type: string
- description: ''
  name: sip
  type: object
- description: ''
  name: icm
  type: object
- description: ''
  name: callRouting
  type: object
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-administration-call-server-config-schema.json
slug: cisco-voice-portal-administration-call-server-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallServerConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serverId\": {\n      \"type\": \"string\"\n    },\n    \"sip\": {\n      \"type\": \"object\"\n    },\n    \"icm\": {\n      \"type\": \"object\"\n    },\n    \"callRouting\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-administration-call-server-config-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: CallServerConfig
---
