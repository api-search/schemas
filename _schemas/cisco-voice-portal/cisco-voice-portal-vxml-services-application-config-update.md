---
description: ''
layout: schema
name: ApplicationConfigUpdate
properties_list:
- description: ''
  name: parameters
  type: object
- description: ''
  name: defaultLanguage
  type: string
- description: ''
  name: fetchTimeout
  type: integer
- description: ''
  name: maxSessionDuration
  type: integer
- description: ''
  name: inputModes
  type: array
- description: ''
  name: loggingLevel
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-application-config-update-schema.json
slug: cisco-voice-portal-vxml-services-application-config-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationConfigUpdate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"parameters\": {\n      \"type\": \"object\"\n    },\n    \"defaultLanguage\": {\n      \"type\": \"string\"\n    },\n    \"fetchTimeout\": {\n      \"type\": \"integer\"\n    },\n    \"maxSessionDuration\": {\n      \"type\": \"integer\"\n    },\n    \"inputModes\": {\n      \"type\": \"array\"\n    },\n    \"loggingLevel\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-application-config-update-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: ApplicationConfigUpdate
---
