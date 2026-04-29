---
description: The result of a log aggregation query.
layout: schema
name: LogAggregateResult
properties_list:
- description: The aggregated log data grouped by the specified dimensions.
  name: results
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/log-monitoring-api-v2-log-aggregate-result-schema.json
slug: log-monitoring-api-v2-log-aggregate-result
source_filename: log-monitoring-api-v2-log-aggregate-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/log-monitoring-api-v2-log-aggregate-result-schema.json\",\n  \"title\": \"LogAggregateResult\",\n  \"description\": \"The result of a log aggregation query.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"The aggregated log data grouped by the specified dimensions.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LogAggregateGroup\"\n      },\n      \"example\": [\n        {\n          \"groupByFields\": {},\n          \"count\": 500\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/log-monitoring-api-v2-log-aggregate-result-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: LogAggregateResult
---
