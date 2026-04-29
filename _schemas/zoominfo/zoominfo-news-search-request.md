---
description: ''
layout: schema
name: NewsSearchRequest
properties_list:
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
  name: page
  type: integer
- description: ''
  name: rpp
  type: integer
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-news-search-request-schema.json
slug: zoominfo-news-search-request
source_filename: zoominfo-news-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"url\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": \"https://www.example.com\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"pageDateMin\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"pageDateMax\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"rpp\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    }\n  },\n  \"required\": [\n    \"categories\",\n    \"url\",\n    \"pageDateMin\",\n    \"pageDateMax\",\n    \"page\",\n    \"rpp\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\"\
  : \"NewsSearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-news-search-request-schema.json
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
title: NewsSearchRequest
---
