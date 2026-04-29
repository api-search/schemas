---
description: ''
layout: schema
name: RealtimeStatistics
properties_list:
- description: ''
  name: timestamp
  type: string
- description: Current number of active calls
  name: activeCalls
  type: integer
- description: ''
  name: callsInProgress
  type: object
- description: Current calls per second rate
  name: callsPerSecond
  type: number
- description: Peak active calls in current period
  name: peakActiveCalls
  type: integer
- description: ''
  name: serverMetrics
  type: array
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-reporting-realtime-statistics-schema.json
slug: cisco-voice-portal-reporting-realtime-statistics
source_filename: cisco-voice-portal-reporting-realtime-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RealtimeStatistics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\"\n    },\n    \"activeCalls\": {\n      \"type\": \"integer\",\n      \"description\": \"Current number of active calls\"\n    },\n    \"callsInProgress\": {\n      \"type\": \"object\"\n    },\n    \"callsPerSecond\": {\n      \"type\": \"number\",\n      \"description\": \"Current calls per second rate\"\n    },\n    \"peakActiveCalls\": {\n      \"type\": \"integer\",\n      \"description\": \"Peak active calls in current period\"\n    },\n    \"serverMetrics\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-reporting-realtime-statistics-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: RealtimeStatistics
---
