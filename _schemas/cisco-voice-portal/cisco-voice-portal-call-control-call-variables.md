---
description: ''
layout: schema
name: CallVariables
properties_list:
- description: ''
  name: callGuid
  type: string
- description: Expanded Call Context variables
  name: eccVariables
  type: object
- description: ICM peripheral variables (1-10)
  name: peripheralVariables
  type: object
- description: ICM call variables (1-10)
  name: callVariables
  type: object
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-call-control-call-variables-schema.json
slug: cisco-voice-portal-call-control-call-variables
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallVariables\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"callGuid\": {\n      \"type\": \"string\"\n    },\n    \"eccVariables\": {\n      \"type\": \"object\",\n      \"description\": \"Expanded Call Context variables\"\n    },\n    \"peripheralVariables\": {\n      \"type\": \"object\",\n      \"description\": \"ICM peripheral variables (1-10)\"\n    },\n    \"callVariables\": {\n      \"type\": \"object\",\n      \"description\": \"ICM call variables (1-10)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-call-control-call-variables-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: CallVariables
---
