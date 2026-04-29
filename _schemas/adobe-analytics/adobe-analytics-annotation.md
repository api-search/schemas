---
description: An annotation marking a date range in reports
layout: schema
name: Annotation
properties_list:
- description: Unique annotation identifier
  name: id
  type: string
- description: Display name of the annotation
  name: name
  type: string
- description: Annotation text content
  name: description
  type: string
- description: ISO 8601 date range covered by this annotation
  name: dateRange
  type: string
- description: List of report suite IDs this annotation applies to
  name: rsids
  type: array
- description: Display color for the annotation in reports
  name: color
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-annotation-schema.json
slug: adobe-analytics-annotation
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An annotation marking a date range in reports\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique annotation identifier\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the annotation\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Annotation text content\",\n      \"example\": \"A sample description.\"\n    },\n    \"dateRange\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 date range covered by this annotation\",\n      \"example\": \"example_value\"\n    },\n    \"rsids\": {\n      \"type\": \"array\",\n      \"description\": \"List of report suite IDs this annotation applies to\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"color\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Display color for the annotation in reports\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Annotation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-annotation-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: Annotation
---
