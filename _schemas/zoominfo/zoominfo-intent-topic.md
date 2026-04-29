---
description: ''
layout: schema
name: IntentTopic
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: Category
  type: string
- description: ''
  name: Department
  type: string
- description: ''
  name: JobFunction
  type: string
- description: ''
  name: Description
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-intent-topic-schema.json
slug: zoominfo-intent-topic
source_filename: zoominfo-intent-topic-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"Category\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Department\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"JobFunction\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"example\": \"Enterprise software company\"\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Category\",\n    \"Department\",\n    \"JobFunction\",\n    \"Description\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IntentTopic\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-intent-topic-schema.json
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
title: IntentTopic
---
