---
description: Payload for creating or updating a calculated metric
layout: schema
name: CalculatedMetricCreate
properties_list:
- description: Display name
  name: name
  type: string
- description: Description of what the metric measures
  name: description
  type: string
- description: Report suite ID
  name: rsid
  type: string
- description: The formula definition
  name: definition
  type: object
- description: The metric output type
  name: type
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-calculated-metric-create-schema.json
slug: adobe-analytics-calculated-metric-create
source_filename: adobe-analytics-calculated-metric-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Payload for creating or updating a calculated metric\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the metric measures\",\n      \"example\": \"A sample description.\"\n    },\n    \"rsid\": {\n      \"type\": \"string\",\n      \"description\": \"Report suite ID\",\n      \"example\": \"500123\"\n    },\n    \"definition\": {\n      \"type\": \"object\",\n      \"description\": \"The formula definition\",\n      \"example\": \"example_value\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The metric output type\",\n      \"example\": \"DECIMAL\",\n      \"enum\": [\n        \"DECIMAL\",\n        \"TIME\",\n        \"PERCENT\",\n        \"CURRENCY\"\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"name\",\n    \"rsid\",\n    \"definition\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CalculatedMetricCreate\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-calculated-metric-create-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: CalculatedMetricCreate
---
