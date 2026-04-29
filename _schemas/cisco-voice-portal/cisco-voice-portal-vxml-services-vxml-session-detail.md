---
description: ''
layout: schema
name: VxmlSessionDetail
properties_list:
- description: ''
  name: sessionId
  type: string
- description: ''
  name: callGuid
  type: string
- description: ''
  name: applicationName
  type: string
- description: ''
  name: startTime
  type: string
- description: ''
  name: duration
  type: integer
- description: ''
  name: currentElement
  type: string
- description: ''
  name: callingNumber
  type: string
- description: ''
  name: calledNumber
  type: string
- description: VXML session-level variables
  name: sessionVariables
  type: object
- description: History of elements visited in this session
  name: elementHistory
  type: array
- description: Last input received from the caller (DTMF or ASR result)
  name: lastUserInput
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-vxml-session-detail-schema.json
slug: cisco-voice-portal-vxml-services-vxml-session-detail
source_filename: cisco-voice-portal-vxml-services-vxml-session-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VxmlSessionDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\"\n    },\n    \"callGuid\": {\n      \"type\": \"string\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"duration\": {\n      \"type\": \"integer\"\n    },\n    \"currentElement\": {\n      \"type\": \"string\"\n    },\n    \"callingNumber\": {\n      \"type\": \"string\"\n    },\n    \"calledNumber\": {\n      \"type\": \"string\"\n    },\n    \"sessionVariables\": {\n      \"type\": \"object\",\n      \"description\": \"VXML session-level variables\"\n    },\n    \"elementHistory\": {\n      \"type\": \"array\",\n      \"description\": \"History of elements visited in this session\"\n    },\n    \"lastUserInput\": {\n      \"type\": \"string\",\n      \"description\": \"Last input received\
  \ from the caller (DTMF or ASR result)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-vxml-session-detail-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: VxmlSessionDetail
---
