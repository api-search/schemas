---
description: ''
layout: schema
name: Input1
properties_list:
- description: ''
  name: companyid
  type: integer
- description: ''
  name: fullname
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-input1-schema.json
slug: zoominfo-input1
source_filename: zoominfo-input1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyid\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"fullname\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    }\n  },\n  \"required\": [\n    \"companyid\",\n    \"fullname\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Input1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-input1-schema.json
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
title: Input1
---
