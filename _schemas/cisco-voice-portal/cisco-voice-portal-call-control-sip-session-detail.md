---
description: ''
layout: schema
name: SipSessionDetail
properties_list:
- description: ''
  name: sessionId
  type: string
- description: ''
  name: callId
  type: string
- description: ''
  name: callGuid
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: fromUri
  type: string
- description: ''
  name: toUri
  type: string
- description: ''
  name: fromTag
  type: string
- description: ''
  name: toTag
  type: string
- description: ''
  name: cseq
  type: integer
- description: ''
  name: transport
  type: string
- description: ''
  name: localAddress
  type: string
- description: ''
  name: remoteAddress
  type: string
- description: ''
  name: startTime
  type: string
- description: ''
  name: lastActivityTime
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-call-control-sip-session-detail-schema.json
slug: cisco-voice-portal-call-control-sip-session-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SipSessionDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\"\n    },\n    \"callId\": {\n      \"type\": \"string\"\n    },\n    \"callGuid\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"fromUri\": {\n      \"type\": \"string\"\n    },\n    \"toUri\": {\n      \"type\": \"string\"\n    },\n    \"fromTag\": {\n      \"type\": \"string\"\n    },\n    \"toTag\": {\n      \"type\": \"string\"\n    },\n    \"cseq\": {\n      \"type\": \"integer\"\n    },\n    \"transport\": {\n      \"type\": \"string\"\n    },\n    \"localAddress\": {\n      \"type\": \"string\"\n    },\n    \"remoteAddress\": {\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"lastActivityTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-call-control-sip-session-detail-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: SipSessionDetail
---
