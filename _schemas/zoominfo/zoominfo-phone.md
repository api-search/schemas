---
description: ''
layout: schema
name: Phone
properties_list:
- description: ''
  name: zi_c_country
  type: string
- description: ''
  name: zi_c_phone
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-phone-schema.json
slug: zoominfo-phone
source_filename: zoominfo-phone-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"zi_c_country\": {\n      \"type\": \"string\",\n      \"example\": \"US\"\n    },\n    \"zi_c_phone\": {\n      \"type\": \"string\",\n      \"example\": \"+1-555-555-1234\"\n    }\n  },\n  \"required\": [\n    \"zi_c_country\",\n    \"zi_c_phone\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Phone\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-phone-schema.json
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
title: Phone
---
