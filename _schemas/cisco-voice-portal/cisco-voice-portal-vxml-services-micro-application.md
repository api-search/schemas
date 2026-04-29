---
description: ''
layout: schema
name: MicroApplication
properties_list:
- description: Micro-application name
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: configurable
  type: boolean
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-micro-application-schema.json
slug: cisco-voice-portal-vxml-services-micro-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MicroApplication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Micro-application name\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"configurable\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-micro-application-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: MicroApplication
---
