---
description: ''
layout: schema
name: ActiveCall
properties_list:
- description: Globally unique call identifier
  name: callGuid
  type: string
- description: ''
  name: state
  type: string
- description: Caller ANI
  name: callingNumber
  type: string
- description: Called DNIS
  name: calledNumber
  type: string
- description: ''
  name: startTime
  type: string
- description: Current call duration in seconds
  name: duration
  type: integer
- description: Current VXML application handling the call
  name: applicationName
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-call-control-active-call-schema.json
slug: cisco-voice-portal-call-control-active-call
source_filename: cisco-voice-portal-call-control-active-call-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ActiveCall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"callGuid\": {\n      \"type\": \"string\",\n      \"description\": \"Globally unique call identifier\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"callingNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Caller ANI\"\n    },\n    \"calledNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Called DNIS\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Current call duration in seconds\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"Current VXML application handling the call\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-call-control-active-call-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: ActiveCall
---
