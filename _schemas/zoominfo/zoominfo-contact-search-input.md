---
description: ''
layout: schema
name: ContactSearchInput
properties_list:
- description: ''
  name: fieldName
  type: string
- description: ''
  name: fieldType
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: accessGranted
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-contact-search-input-schema.json
slug: zoominfo-contact-search-input
source_filename: zoominfo-contact-search-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"fieldType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"Enterprise software company\"\n    },\n    \"accessGranted\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"fieldName\",\n    \"fieldType\",\n    \"description\",\n    \"accessGranted\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactSearchInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-contact-search-input-schema.json
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
title: ContactSearchInput
---
