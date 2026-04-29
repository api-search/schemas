---
description: Summary metric value containing statistical aggregations
layout: schema
name: SummaryValue
properties_list:
- description: The number of measurements in this summary
  name: count
  type: number
- description: The sum of all measurement values
  name: sum
  type: number
- description: The minimum measurement value
  name: min
  type: number
- description: The maximum measurement value
  name: max
  type: number
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/metric-api-summary-value-schema.json
slug: metric-api-summary-value
source_filename: metric-api-summary-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/metric-api-summary-value-schema.json\",\n  \"title\": \"SummaryValue\",\n  \"description\": \"Summary metric value containing statistical aggregations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"number\",\n      \"description\": \"The number of measurements in this summary\",\n      \"example\": 42.5\n    },\n    \"sum\": {\n      \"type\": \"number\",\n      \"description\": \"The sum of all measurement values\",\n      \"example\": 42.5\n    },\n    \"min\": {\n      \"type\": \"number\",\n      \"description\": \"The minimum measurement value\",\n      \"example\": 42.5\n    },\n    \"max\": {\n      \"type\": \"number\",\n      \"description\": \"The maximum measurement value\",\n      \"example\": 42.5\n    }\n  },\n  \"required\": [\n    \"count\",\n    \"sum\"\
  ,\n    \"min\",\n    \"max\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/metric-api-summary-value-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: SummaryValue
---
