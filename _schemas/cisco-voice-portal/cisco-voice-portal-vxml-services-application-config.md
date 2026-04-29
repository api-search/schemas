---
description: ''
layout: schema
name: ApplicationConfig
properties_list:
- description: ''
  name: applicationName
  type: string
- description: Runtime configuration parameters
  name: parameters
  type: object
- description: ''
  name: defaultLanguage
  type: string
- description: VXML document fetch timeout in milliseconds
  name: fetchTimeout
  type: integer
- description: Maximum session duration in seconds
  name: maxSessionDuration
  type: integer
- description: Allowed input modes
  name: inputModes
  type: array
- description: ''
  name: loggingLevel
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-application-config-schema.json
slug: cisco-voice-portal-vxml-services-application-config
source_filename: cisco-voice-portal-vxml-services-application-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Runtime configuration parameters\"\n    },\n    \"defaultLanguage\": {\n      \"type\": \"string\"\n    },\n    \"fetchTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"VXML document fetch timeout in milliseconds\"\n    },\n    \"maxSessionDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum session duration in seconds\"\n    },\n    \"inputModes\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed input modes\"\n    },\n    \"loggingLevel\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-application-config-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: ApplicationConfig
---
