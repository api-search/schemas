---
description: ''
layout: schema
name: Usage
properties_list:
- description: ''
  name: usage
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-usage-schema.json
slug: zoominfo-usage
source_filename: zoominfo-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"usage\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"limitType\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"Enterprise software company\"\n          },\n          \"limit\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          },\n          \"currentUsage\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          },\n          \"usageRemaining\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          }\n        },\n        \"required\": [\n          \"limitType\",\n          \"description\",\n          \"limit\",\n          \"currentUsage\",\n          \"usageRemaining\"\n        ]\n\
  \      }\n    }\n  },\n  \"required\": [\n    \"usage\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Usage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-usage-schema.json
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
title: Usage
---
