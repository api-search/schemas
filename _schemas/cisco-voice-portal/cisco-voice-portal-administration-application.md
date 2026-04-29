---
description: ''
layout: schema
name: Application
properties_list:
- description: ''
  name: applicationId
  type: string
- description: ''
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
- description: ''
  name: deployedServers
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-administration-application-schema.json
slug: cisco-voice-portal-administration-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"type\": \"string\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\"\n    },\n    \"applicationType\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"deployedServers\": {\n      \"type\": \"array\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-administration-application-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: Application
---
