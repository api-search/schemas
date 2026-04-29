---
description: ''
layout: schema
name: Matchbycompanyaddress1
properties_list:
- description: ''
  name: responseCode
  type: integer
- description: ''
  name: message
  type: string
- description: ''
  name: invalidOutputFields
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-matchbycompanyaddress1-schema.json
slug: zoominfo-matchbycompanyaddress1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"responseCode\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"invalidOutputFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"responseCode\",\n    \"message\",\n    \"invalidOutputFields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Matchbycompanyaddress1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-matchbycompanyaddress1-schema.json
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
title: Matchbycompanyaddress1
---
