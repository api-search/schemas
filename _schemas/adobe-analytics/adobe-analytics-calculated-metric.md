---
description: A calculated metric definition
layout: schema
name: CalculatedMetric
properties_list:
- description: Unique calculated metric identifier
  name: id
  type: string
- description: Display name
  name: name
  type: string
- description: Description of what the metric measures
  name: description
  type: string
- description: The report suite this calculated metric is based on
  name: rsid
  type: string
- description: The owner of an Analytics component
  name: owner
  type: object
- description: The formula definition for this calculated metric
  name: definition
  type: object
- description: Last modification timestamp
  name: modified
  type: string
- description: The metric type
  name: type
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-calculated-metric-schema.json
slug: adobe-analytics-calculated-metric
source_filename: adobe-analytics-calculated-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A calculated metric definition\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique calculated metric identifier\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the metric measures\",\n      \"example\": \"A sample description.\"\n    },\n    \"rsid\": {\n      \"type\": \"string\",\n      \"description\": \"The report suite this calculated metric is based on\",\n      \"example\": \"500123\"\n    },\n    \"owner\": {\n      \"type\": \"object\",\n      \"description\": \"The owner of an Analytics component\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Owner user ID\",\n          \"example\"\
  : \"abc123\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Owner display name\",\n          \"example\": \"Example Title\"\n        },\n        \"login\": {\n          \"type\": \"string\",\n          \"description\": \"Owner login identifier\",\n          \"example\": \"example_value\"\n        }\n      }\n    },\n    \"definition\": {\n      \"type\": \"object\",\n      \"description\": \"The formula definition for this calculated metric\",\n      \"example\": \"example_value\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"description\": \"Last modification timestamp\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The metric type\",\n      \"example\": \"DECIMAL\",\n      \"enum\": [\n        \"DECIMAL\",\n        \"TIME\",\n        \"PERCENT\",\n        \"CURRENCY\"\n      ]\n    }\n  },\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CalculatedMetric\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-calculated-metric-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: CalculatedMetric
---
