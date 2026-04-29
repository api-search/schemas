---
description: ''
layout: schema
name: VxmlServerStatus
properties_list:
- description: ''
  name: hostname
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: uptime
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: activeSessions
  type: integer
- description: ''
  name: maxSessions
  type: integer
- description: ''
  name: threadPool
  type: object
- description: ''
  name: cpuUsage
  type: number
- description: ''
  name: memoryUsage
  type: object
- description: ''
  name: deployedApplications
  type: integer
- description: ''
  name: timestamp
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-vxml-server-status-schema.json
slug: cisco-voice-portal-vxml-services-vxml-server-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VxmlServerStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hostname\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"uptime\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"activeSessions\": {\n      \"type\": \"integer\"\n    },\n    \"maxSessions\": {\n      \"type\": \"integer\"\n    },\n    \"threadPool\": {\n      \"type\": \"object\"\n    },\n    \"cpuUsage\": {\n      \"type\": \"number\"\n    },\n    \"memoryUsage\": {\n      \"type\": \"object\"\n    },\n    \"deployedApplications\": {\n      \"type\": \"integer\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-vxml-server-status-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: VxmlServerStatus
---
