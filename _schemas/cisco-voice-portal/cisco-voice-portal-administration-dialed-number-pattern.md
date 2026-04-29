---
description: ''
layout: schema
name: DialedNumberPattern
properties_list:
- description: ''
  name: patternId
  type: string
- description: 'The dialed number pattern (supports wildcards). Example: 1800555*'
  name: pattern
  type: string
- description: ''
  name: description
  type: string
- description: Call type for ICM routing
  name: callType
  type: string
- description: Associated VXML application name
  name: applicationName
  type: string
- description: ''
  name: enabled
  type: boolean
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-administration-dialed-number-pattern-schema.json
slug: cisco-voice-portal-administration-dialed-number-pattern
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DialedNumberPattern\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"patternId\": {\n      \"type\": \"string\"\n    },\n    \"pattern\": {\n      \"type\": \"string\",\n      \"description\": \"The dialed number pattern (supports wildcards). Example: 1800555*\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"callType\": {\n      \"type\": \"string\",\n      \"description\": \"Call type for ICM routing\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"Associated VXML application name\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-administration-dialed-number-pattern-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: DialedNumberPattern
---
