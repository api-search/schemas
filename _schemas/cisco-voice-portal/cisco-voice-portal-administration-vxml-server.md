---
description: ''
layout: schema
name: VxmlServer
properties_list:
- description: ''
  name: serverId
  type: string
- description: ''
  name: hostname
  type: string
- description: ''
  name: ipAddress
  type: string
- description: ''
  name: httpPort
  type: integer
- description: ''
  name: httpsPort
  type: integer
- description: ''
  name: status
  type: string
- description: Number of applications deployed on this server
  name: deployedApplications
  type: integer
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-administration-vxml-server-schema.json
slug: cisco-voice-portal-administration-vxml-server
source_filename: cisco-voice-portal-administration-vxml-server-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VxmlServer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serverId\": {\n      \"type\": \"string\"\n    },\n    \"hostname\": {\n      \"type\": \"string\"\n    },\n    \"ipAddress\": {\n      \"type\": \"string\"\n    },\n    \"httpPort\": {\n      \"type\": \"integer\"\n    },\n    \"httpsPort\": {\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"deployedApplications\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of applications deployed on this server\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-administration-vxml-server-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: VxmlServer
---
