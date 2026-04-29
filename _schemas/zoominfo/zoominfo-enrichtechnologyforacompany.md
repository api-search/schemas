---
description: ''
layout: schema
name: Enrichtechnologyforacompany
properties_list:
- description: ''
  name: maxResults
  type: integer
- description: ''
  name: totalResults
  type: integer
- description: ''
  name: currentPage
  type: integer
- description: ''
  name: data
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-enrichtechnologyforacompany-schema.json
slug: zoominfo-enrichtechnologyforacompany
source_filename: zoominfo-enrichtechnologyforacompany-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"currentPage\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"tag\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"categoryParent\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"vendor\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"product\": {\n\
  \            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"attribute\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"website\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"logo\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"domain\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"createdTime\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"modifiedTime\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"Enterprise software company\"\n          }\n        },\n\
  \        \"required\": [\n          \"tag\",\n          \"categoryParent\",\n          \"category\",\n          \"vendor\",\n          \"product\",\n          \"attribute\",\n          \"website\",\n          \"logo\",\n          \"domain\",\n          \"createdTime\",\n          \"modifiedTime\",\n          \"description\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"maxResults\",\n    \"totalResults\",\n    \"currentPage\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Enrichtechnologyforacompany\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-enrichtechnologyforacompany-schema.json
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
title: Enrichtechnologyforacompany
---
