---
description: ''
layout: schema
name: MicroAppConfig
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Configuration parameters for the micro-application
  name: parameters
  type: array
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-micro-app-config-schema.json
slug: cisco-voice-portal-vxml-services-micro-app-config
source_filename: cisco-voice-portal-vxml-services-micro-app-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MicroAppConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"Configuration parameters for the micro-application\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-micro-app-config-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: MicroAppConfig
---
