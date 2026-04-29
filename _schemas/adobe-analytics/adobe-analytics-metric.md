---
description: An analytics metric available in a report suite
layout: schema
name: Metric
properties_list:
- description: Metric ID (e.g. metrics/visits)
  name: id
  type: string
- description: Display name of the metric
  name: title
  type: string
- description: Internal name
  name: name
  type: string
- description: Metric data type
  name: type
  type: string
- description: Additional context for the metric title
  name: extraTitleInfo
  type: string
- description: Category grouping for the metric
  name: category
  type: string
- description: Description of what the metric measures
  name: description
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-metric-schema.json
slug: adobe-analytics-metric
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An analytics metric available in a report suite\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Metric ID (e.g. metrics/visits)\",\n      \"example\": \"abc123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the metric\",\n      \"example\": \"Example Title\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name\",\n      \"example\": \"Example Title\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Metric data type\",\n      \"example\": \"INT\",\n      \"enum\": [\n        \"INT\",\n        \"DECIMAL\",\n        \"CURRENCY\",\n        \"PERCENT\",\n        \"TIME\"\n      ]\n    },\n    \"extraTitleInfo\": {\n      \"type\": \"string\",\n      \"description\": \"Additional context for the metric title\",\n      \"example\": \"example_value\"\n    },\n    \"\
  category\": {\n      \"type\": \"string\",\n      \"description\": \"Category grouping for the metric\",\n      \"example\": \"example_value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the metric measures\",\n      \"example\": \"A sample description.\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Metric\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-metric-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: Metric
---
