---
description: ''
layout: schema
name: CallLeg
properties_list:
- description: ''
  name: legId
  type: string
- description: ''
  name: callGuid
  type: string
- description: Type of call leg
  name: legType
  type: string
- description: ''
  name: startTime
  type: string
- description: ''
  name: endTime
  type: string
- description: Leg duration in seconds
  name: duration
  type: integer
- description: SIP From URI
  name: fromUri
  type: string
- description: SIP To URI
  name: toUri
  type: string
- description: Server that handled this leg
  name: serverHostname
  type: string
- description: Final SIP response code for this leg
  name: sipResponseCode
  type: integer
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-reporting-call-leg-schema.json
slug: cisco-voice-portal-reporting-call-leg
source_filename: cisco-voice-portal-reporting-call-leg-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallLeg\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"legId\": {\n      \"type\": \"string\"\n    },\n    \"callGuid\": {\n      \"type\": \"string\"\n    },\n    \"legType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of call leg\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"endTime\": {\n      \"type\": \"string\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Leg duration in seconds\"\n    },\n    \"fromUri\": {\n      \"type\": \"string\",\n      \"description\": \"SIP From URI\"\n    },\n    \"toUri\": {\n      \"type\": \"string\",\n      \"description\": \"SIP To URI\"\n    },\n    \"serverHostname\": {\n      \"type\": \"string\",\n      \"description\": \"Server that handled this leg\"\n    },\n    \"sipResponseCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Final SIP response\
  \ code for this leg\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-reporting-call-leg-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: CallLeg
---
