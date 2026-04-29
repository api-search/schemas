---
description: ''
layout: schema
name: LogEntry
properties_list:
- description: ''
  name: timestamp
  type: string
- description: ''
  name: level
  type: string
- description: ''
  name: logger
  type: string
- description: ''
  name: message
  type: string
- description: Associated session ID, if applicable
  name: sessionId
  type: string
- description: Associated application, if applicable
  name: applicationName
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-vxml-services-log-entry-schema.json
slug: cisco-voice-portal-vxml-services-log-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogEntry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\"\n    },\n    \"level\": {\n      \"type\": \"string\"\n    },\n    \"logger\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated session ID, if applicable\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"Associated application, if applicable\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-vxml-services-log-entry-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: LogEntry
---
