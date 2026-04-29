---
description: ''
layout: schema
name: CallSummaryStatistics
properties_list:
- description: ''
  name: startTime
  type: string
- description: ''
  name: endTime
  type: string
- description: ''
  name: interval
  type: string
- description: ''
  name: intervals
  type: array
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-reporting-call-summary-statistics-schema.json
slug: cisco-voice-portal-reporting-call-summary-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CallSummaryStatistics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"startTime\": {\n      \"type\": \"string\"\n    },\n    \"endTime\": {\n      \"type\": \"string\"\n    },\n    \"interval\": {\n      \"type\": \"string\"\n    },\n    \"intervals\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-reporting-call-summary-statistics-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: CallSummaryStatistics
---
