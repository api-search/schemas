---
description: ''
layout: schema
name: ExternalUrl
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: url
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-external-url-schema.json
slug: zoominfo-external-url
source_filename: zoominfo-external-url-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com/resource\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExternalUrl\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-external-url-schema.json
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
title: ExternalUrl
---
