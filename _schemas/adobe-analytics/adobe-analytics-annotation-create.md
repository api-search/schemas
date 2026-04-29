---
description: Payload for creating an annotation
layout: schema
name: AnnotationCreate
properties_list:
- description: Display name
  name: name
  type: string
- description: Annotation notes
  name: description
  type: string
- description: ISO 8601 date range
  name: dateRange
  type: string
- description: Report suite IDs to apply to
  name: rsids
  type: array
- description: Hex color code
  name: color
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-annotation-create-schema.json
slug: adobe-analytics-annotation-create
source_filename: adobe-analytics-annotation-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Payload for creating an annotation\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Annotation notes\",\n      \"example\": \"A sample description.\"\n    },\n    \"dateRange\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 date range\",\n      \"example\": \"example_value\"\n    },\n    \"rsids\": {\n      \"type\": \"array\",\n      \"description\": \"Report suite IDs to apply to\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"Hex color code\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"dateRange\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"AnnotationCreate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-annotation-create-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: AnnotationCreate
---
