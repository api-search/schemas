---
description: ''
layout: schema
name: IntentEnrichRequest
properties_list:
- description: ''
  name: companyName
  type: string
- description: ''
  name: companyWebsite
  type: string
- description: ''
  name: companyId
  type: integer
- description: ''
  name: topics
  type: array
- description: ''
  name: signalStartDate
  type: string
- description: ''
  name: signalEndDate
  type: string
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
  name: sortBy
  type: string
- description: ''
  name: sortOrder
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-intent-enrich-request-schema.json
slug: zoominfo-intent-enrich-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"companyWebsite\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"companyId\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"signalStartDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"signalEndDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"signalScoreMin\": {\n      \"type\": \"integer\",\n      \"example\": 85\n    },\n    \"signalScoreMax\": {\n      \"type\": \"integer\",\n      \"example\": 85\n    },\n    \"audienceStrengthMin\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\
  \n    },\n    \"audienceStrengthMax\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sortBy\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sortOrder\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"companyName\",\n    \"companyWebsite\",\n    \"companyId\",\n    \"topics\",\n    \"signalStartDate\",\n    \"signalEndDate\",\n    \"signalScoreMin\",\n    \"signalScoreMax\",\n    \"audienceStrengthMin\",\n    \"audienceStrengthMax\",\n    \"sortBy\",\n    \"sortOrder\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntentEnrichRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-intent-enrich-request-schema.json
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
title: IntentEnrichRequest
---
