---
description: ''
layout: schema
name: NewsEnrichRequest
properties_list:
- description: ''
  name: companyId
  type: integer
- description: ''
  name: categories
  type: array
- description: ''
  name: url
  type: array
- description: ''
  name: pageDateMin
  type: string
- description: ''
  name: pageDateMax
  type: string
- description: ''
  name: limit
  type: integer
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-news-enrich-request-schema.json
slug: zoominfo-news-enrich-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"url\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": \"https://www.example.com\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"pageDateMin\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"pageDateMax\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    }\n  },\n  \"required\": [\n    \"companyId\",\n    \"categories\",\n    \"url\",\n    \"pageDateMin\",\n    \"pageDateMax\",\n    \"limit\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"NewsEnrichRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-news-enrich-request-schema.json
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
title: NewsEnrichRequest
---
