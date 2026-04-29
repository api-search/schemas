---
description: ''
layout: schema
name: CdrQueryResult
properties_list:
- description: Total number of matching records
  name: totalRecords
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: limit
  type: integer
- description: ''
  name: records
  type: array
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-reporting-cdr-query-result-schema.json
slug: cisco-voice-portal-reporting-cdr-query-result
source_filename: cisco-voice-portal-reporting-cdr-query-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CdrQueryResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalRecords\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching records\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"records\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-reporting-cdr-query-result-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: CdrQueryResult
---
