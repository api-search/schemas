---
description: ''
layout: schema
name: ScoopSearchRequest
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
  name: updatedSinceCreation
  type: boolean
- description: ''
  name: description
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-scoop-search-request-schema.json
slug: zoominfo-scoop-search-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"publishedStartDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"publishedEndDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"scoopType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"updatedSinceCreation\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Enterprise software company\"\n    }\n  },\n  \"required\": [\n    \"companyName\",\n    \"publishedStartDate\",\n    \"publishedEndDate\",\n    \"scoopType\",\n    \"updatedSinceCreation\",\n    \"description\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScoopSearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-scoop-search-request-schema.json
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
title: ScoopSearchRequest
---
