---
description: ''
layout: schema
name: Input9
properties_list:
- description: ''
  name: address
  type: object
- description: ''
  name: match_reasons
  type: array
- description: ''
  name: zi_c_name
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-input9-schema.json
slug: zoominfo-input9
source_filename: zoominfo-input9-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"zi_c_city\": {\n          \"type\": \"string\",\n          \"example\": \"San Francisco\"\n        },\n        \"zi_c_country\": {\n          \"type\": \"string\",\n          \"example\": \"US\"\n        },\n        \"zi_c_state\": {\n          \"type\": \"string\",\n          \"example\": \"CA\"\n        },\n        \"zi_c_zip\": {\n          \"type\": \"string\",\n          \"example\": \"94105\"\n        }\n      },\n      \"required\": [\n        \"zi_c_city\",\n        \"zi_c_country\",\n        \"zi_c_state\",\n        \"zi_c_zip\"\n      ]\n    },\n    \"match_reasons\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"zi_c_name\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\
  \n          }\n        },\n        \"required\": [\n          \"zi_c_name\"\n        ]\n      }\n    },\n    \"zi_c_name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    }\n  },\n  \"required\": [\n    \"address\",\n    \"match_reasons\",\n    \"zi_c_name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Input9\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-input9-schema.json
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
title: Input9
---
