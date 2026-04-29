---
description: ''
layout: schema
name: HealthStatus
properties_list:
- description: ''
  name: serverName
  type: string
- description: ''
  name: status
  type: string
- description: Server uptime duration
  name: uptime
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: activeCalls
  type: integer
- description: Maximum concurrent call capacity
  name: maxCalls
  type: integer
- description: ''
  name: sipStackStatus
  type: string
- description: ''
  name: cpuUsage
  type: number
- description: ''
  name: memoryUsage
  type: number
- description: ''
  name: timestamp
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-call-control-health-status-schema.json
slug: cisco-voice-portal-call-control-health-status
source_filename: cisco-voice-portal-call-control-health-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HealthStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serverName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"uptime\": {\n      \"type\": \"string\",\n      \"description\": \"Server uptime duration\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    },\n    \"activeCalls\": {\n      \"type\": \"integer\"\n    },\n    \"maxCalls\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum concurrent call capacity\"\n    },\n    \"sipStackStatus\": {\n      \"type\": \"string\"\n    },\n    \"cpuUsage\": {\n      \"type\": \"number\"\n    },\n    \"memoryUsage\": {\n      \"type\": \"number\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-call-control-health-status-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: HealthStatus
---
