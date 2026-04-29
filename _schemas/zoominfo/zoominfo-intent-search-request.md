---
description: ''
layout: schema
name: IntentSearchRequest
properties_list:
- description: ''
  name: topics
  type: array
- description: ''
  name: signalScoreMin
  type: integer
- description: ''
  name: signalScoreMax
  type: integer
- description: ''
  name: audienceStrengthMin
  type: string
- description: ''
  name: audienceStrengthMax
  type: string
- description: ''
  name: metroRegion
  type: string
- description: ''
  name: industryCodes
  type: string
- description: ''
  name: sortBy
  type: string
- description: ''
  name: sortOrder
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-intent-search-request-schema.json
slug: zoominfo-intent-search-request
source_filename: zoominfo-intent-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"topics\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"signalScoreMin\": {\n      \"type\": \"integer\",\n      \"example\": 85\n    },\n    \"signalScoreMax\": {\n      \"type\": \"integer\",\n      \"example\": 85\n    },\n    \"audienceStrengthMin\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"audienceStrengthMax\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"metroRegion\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"industryCodes\": {\n      \"type\": \"string\",\n      \"example\": \"Software\"\n    },\n    \"sortBy\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sortOrder\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n  \
  \  }\n  },\n  \"required\": [\n    \"topics\",\n    \"signalScoreMin\",\n    \"signalScoreMax\",\n    \"audienceStrengthMin\",\n    \"audienceStrengthMax\",\n    \"metroRegion\",\n    \"industryCodes\",\n    \"sortBy\",\n    \"sortOrder\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntentSearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-intent-search-request-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: IntentSearchRequest
---
