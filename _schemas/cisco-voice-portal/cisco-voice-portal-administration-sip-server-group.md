---
description: ''
layout: schema
name: SipServerGroup
properties_list:
- description: ''
  name: groupId
  type: string
- description: ''
  name: groupName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: servers
  type: array
- description: ''
  name: loadBalancing
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-administration-sip-server-group-schema.json
slug: cisco-voice-portal-administration-sip-server-group
source_filename: cisco-voice-portal-administration-sip-server-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SipServerGroup\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupId\": {\n      \"type\": \"string\"\n    },\n    \"groupName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"servers\": {\n      \"type\": \"array\"\n    },\n    \"loadBalancing\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-administration-sip-server-group-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: SipServerGroup
---
