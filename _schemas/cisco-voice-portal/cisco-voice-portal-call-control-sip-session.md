---
description: ''
layout: schema
name: SipSession
properties_list:
- description: ''
  name: sessionId
  type: string
- description: SIP Call-ID
  name: callId
  type: string
- description: Associated CVP call GUID
  name: callGuid
  type: string
- description: ''
  name: state
  type: string
- description: Initial SIP method (INVITE)
  name: method
  type: string
- description: ''
  name: fromUri
  type: string
- description: ''
  name: toUri
  type: string
- description: ''
  name: startTime
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-call-control-sip-session-schema.json
slug: cisco-voice-portal-call-control-sip-session
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SipSession\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\"\n    },\n    \"callId\": {\n      \"type\": \"string\",\n      \"description\": \"SIP Call-ID\"\n    },\n    \"callGuid\": {\n      \"type\": \"string\",\n      \"description\": \"Associated CVP call GUID\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"description\": \"Initial SIP method (INVITE)\"\n    },\n    \"fromUri\": {\n      \"type\": \"string\"\n    },\n    \"toUri\": {\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-call-control-sip-session-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: SipSession
---
