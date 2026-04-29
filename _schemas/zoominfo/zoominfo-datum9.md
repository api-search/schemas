---
description: ''
layout: schema
name: Datum9
properties_list:
- description: ''
  name: domain
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: imageUrl
  type: string
- description: ''
  name: pageDate
  type: string
- description: ''
  name: categories
  type: array
- description: ''
  name: company
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-datum9-schema.json
slug: zoominfo-datum9
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"example\": \"example.com\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"Vice President of Sales\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com/resource\"\n    },\n    \"imageUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com/resource\"\n    },\n    \"pageDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"company\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n      \
  \      \"example\": 500123\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"name\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"domain\",\n    \"title\",\n    \"url\",\n    \"pageDate\",\n    \"categories\",\n    \"company\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Datum9\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-datum9-schema.json
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
title: Datum9
---
