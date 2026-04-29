---
description: ''
layout: schema
name: Usage1
properties_list:
- description: ''
  name: limitType
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: limit
  type: integer
- description: ''
  name: currentUsage
  type: integer
- description: ''
  name: usageRemaining
  type: integer
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-usage1-schema.json
slug: zoominfo-usage1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"limitType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Enterprise software company\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"currentUsage\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"usageRemaining\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    }\n  },\n  \"required\": [\n    \"limitType\",\n    \"description\",\n    \"limit\",\n    \"currentUsage\",\n    \"usageRemaining\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Usage1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-usage1-schema.json
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
title: Usage1
---
