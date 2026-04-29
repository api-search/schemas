---
description: ''
layout: schema
name: SipServerGroupCreate
properties_list:
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
schema_file: json-schema/cisco-voice-portal-administration-sip-server-group-create-schema.json
slug: cisco-voice-portal-administration-sip-server-group-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SipServerGroupCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"servers\": {\n      \"type\": \"array\"\n    },\n    \"loadBalancing\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-administration-sip-server-group-create-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: SipServerGroupCreate
---
