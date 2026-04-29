---
description: ''
layout: schema
name: VxmlSession
properties_list:
- description: ''
  name: sessionId
  type: string
- description: Associated CVP call GUID
  name: callGuid
  type: string
- description: ''
  name: applicationName
  type: string
- description: ''
  name: startTime
  type: string
- description: Session duration in seconds
  name: duration
  type: integer
- description: Currently executing call flow element
  name: currentElement
  type: string
- description: ''
  name: callingNumber
  type: string
- description: ''
  name: calledNumber
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-vxml-session-schema.json
slug: cisco-voice-portal-vxml-services-vxml-session
source_filename: cisco-voice-portal-vxml-services-vxml-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VxmlSession\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\"\n    },\n    \"callGuid\": {\n      \"type\": \"string\",\n      \"description\": \"Associated CVP call GUID\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Session duration in seconds\"\n    },\n    \"currentElement\": {\n      \"type\": \"string\",\n      \"description\": \"Currently executing call flow element\"\n    },\n    \"callingNumber\": {\n      \"type\": \"string\"\n    },\n    \"calledNumber\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-vxml-session-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: VxmlSession
---
