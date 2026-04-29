---
description: ''
layout: schema
name: ScoopEnrichRequest
properties_list:
- description: ''
  name: companyName
  type: string
- description: ''
  name: publishedStartDate
  type: string
- description: ''
  name: publishedEndDate
  type: string
- description: ''
  name: scoopType
  type: string
- description: ''
  name: department
  type: string
- description: ''
  name: sortBy
  type: string
- description: ''
  name: sortOrder
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-scoop-enrich-request-schema.json
slug: zoominfo-scoop-enrich-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"publishedStartDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"publishedEndDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"scoopType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sortBy\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"sortOrder\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"companyName\",\n    \"publishedStartDate\",\n    \"publishedEndDate\",\n    \"scoopType\",\n    \"department\",\n    \"sortBy\",\n    \"sortOrder\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"ScoopEnrichRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-scoop-enrich-request-schema.json
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
title: ScoopEnrichRequest
---
