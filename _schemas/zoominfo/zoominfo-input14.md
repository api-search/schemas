---
description: ''
layout: schema
name: Input14
properties_list:
- description: ''
  name: zi_c_location_id
  type: integer
- description: ''
  name: address
  type: object
- description: ''
  name: zi_c_url
  type: string
- description: ''
  name: phone
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-input14-schema.json
slug: zoominfo-input14
source_filename: zoominfo-input14-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"zi_c_location_id\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"zi_c_country\": {\n          \"type\": \"string\",\n          \"example\": \"US\"\n        },\n        \"zi_c_state\": {\n          \"type\": \"string\",\n          \"example\": \"CA\"\n        }\n      },\n      \"required\": [\n        \"zi_c_country\",\n        \"zi_c_state\"\n      ]\n    },\n    \"zi_c_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com/resource\"\n    },\n    \"phone\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"zi_c_country\": {\n          \"type\": \"string\",\n          \"example\": \"US\"\n        },\n        \"zi_c_phone\": {\n          \"type\": \"string\",\n          \"example\": \"+1-555-555-1234\"\n        }\n      },\n      \"required\": [\n        \"zi_c_country\"\
  ,\n        \"zi_c_phone\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Input14\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-input14-schema.json
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
title: Input14
---
