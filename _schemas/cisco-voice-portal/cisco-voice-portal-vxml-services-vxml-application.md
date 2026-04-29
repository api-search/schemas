---
description: ''
layout: schema
name: VxmlApplication
properties_list:
- description: Application name
  name: applicationName
  type: string
- description: ''
  name: applicationType
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: version
  type: string
- description: Number of active call sessions
  name: activeSessions
  type: integer
- description: ''
  name: deployedAt
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-vxml-application-schema.json
slug: cisco-voice-portal-vxml-services-vxml-application
source_filename: cisco-voice-portal-vxml-services-vxml-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VxmlApplication\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"Application name\"\n    },\n    \"applicationType\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"activeSessions\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of active call sessions\"\n    },\n    \"deployedAt\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-vxml-application-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: VxmlApplication
---
