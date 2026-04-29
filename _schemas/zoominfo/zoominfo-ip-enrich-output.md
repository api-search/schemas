---
description: ''
layout: schema
name: IPEnrichOutput
properties_list:
- description: ''
  name: fieldName
  type: string
- description: ''
  name: description
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-ip-enrich-output-schema.json
slug: zoominfo-ip-enrich-output
source_filename: zoominfo-ip-enrich-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Enterprise software company\"\n    }\n  },\n  \"required\": [\n    \"fieldName\",\n    \"description\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IPEnrichOutput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-ip-enrich-output-schema.json
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
title: IPEnrichOutput
---
