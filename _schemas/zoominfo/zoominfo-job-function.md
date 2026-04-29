---
description: ''
layout: schema
name: JobFunction
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: department
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-job-function-schema.json
slug: zoominfo-job-function
source_filename: zoominfo-job-function-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"department\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobFunction\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-job-function-schema.json
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
title: JobFunction
---
