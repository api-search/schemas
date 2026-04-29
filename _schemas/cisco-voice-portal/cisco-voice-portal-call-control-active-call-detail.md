---
description: ''
layout: schema
name: ActiveCallDetail
properties_list:
- description: ''
  name: callGuid
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: callingNumber
  type: string
- description: ''
  name: calledNumber
  type: string
- description: ''
  name: startTime
  type: string
- description: ''
  name: duration
  type: integer
- description: ''
  name: applicationName
  type: string
- description: SIP Call-ID
  name: sipCallId
  type: string
- description: ''
  name: sipFromTag
  type: string
- description: ''
  name: sipToTag
  type: string
- description: ''
  name: icmRouteResult
  type: object
- description: VXML Server currently handling the call
  name: vxmlServer
  type: string
- description: Chronological list of call events
  name: callHistory
  type: array
- description: ''
  name: eccVariables
  type: object
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-call-control-active-call-detail-schema.json
slug: cisco-voice-portal-call-control-active-call-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActiveCallDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"callGuid\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"callingNumber\": {\n      \"type\": \"string\"\n    },\n    \"calledNumber\": {\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"duration\": {\n      \"type\": \"integer\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\"\n    },\n    \"sipCallId\": {\n      \"type\": \"string\",\n      \"description\": \"SIP Call-ID\"\n    },\n    \"sipFromTag\": {\n      \"type\": \"string\"\n    },\n    \"sipToTag\": {\n      \"type\": \"string\"\n    },\n    \"icmRouteResult\": {\n      \"type\": \"object\"\n    },\n    \"vxmlServer\": {\n      \"type\": \"string\",\n      \"description\": \"VXML Server currently handling the call\"\n    },\n    \"callHistory\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Chronological list of call events\"\n    },\n    \"eccVariables\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-call-control-active-call-detail-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: ActiveCallDetail
---
