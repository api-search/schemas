---
description: ''
layout: schema
name: Competitor
properties_list:
- description: ''
  name: rank
  type: integer
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: website
  type: string
- description: ''
  name: employeeCount
  type: integer
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-competitor-schema.json
slug: zoominfo-competitor
source_filename: zoominfo-competitor-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"rank\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"employeeCount\": {\n      \"type\": \"integer\",\n      \"example\": 250\n    }\n  },\n  \"required\": [\n    \"rank\",\n    \"id\",\n    \"name\",\n    \"website\",\n    \"employeeCount\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Competitor\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-competitor-schema.json
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
title: Competitor
---
