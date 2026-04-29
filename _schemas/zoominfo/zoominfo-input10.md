---
description: ''
layout: schema
name: Input10
properties_list:
- description: ''
  name: phone
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-input10-schema.json
slug: zoominfo-input10
source_filename: zoominfo-input10-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"phone\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"zi_c_country\": {\n          \"type\": \"string\",\n          \"example\": \"US\"\n        },\n        \"zi_c_phone\": {\n          \"type\": \"string\",\n          \"example\": \"+1-555-555-1234\"\n        }\n      },\n      \"required\": [\n        \"zi_c_country\",\n        \"zi_c_phone\"\n      ]\n    }\n  },\n  \"required\": [\n    \"phone\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Input10\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-input10-schema.json
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
title: Input10
---
