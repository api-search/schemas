---
description: ''
layout: schema
name: ConnectivityStatus
properties_list:
- description: ''
  name: timestamp
  type: string
- description: ''
  name: connections
  type: array
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-call-control-connectivity-status-schema.json
slug: cisco-voice-portal-call-control-connectivity-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConnectivityStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\"\n    },\n    \"connections\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-call-control-connectivity-status-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: ConnectivityStatus
---
