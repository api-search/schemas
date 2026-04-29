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
schema_file: json-schema/dynatrace-log-monitoring-v2-log-aggregate-result-schema.json
slug: dynatrace-log-monitoring-v2-log-aggregate-result
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result of a log aggregation query.\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"The aggregated log data grouped by the specified dimensions.\",\n      \"example\": [\n        {\n          \"groupByFields\": {},\n          \"count\": 500\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single aggregation group result.\",\n        \"properties\": {\n          \"groupByFields\": {\n            \"type\": \"object\",\n            \"description\": \"The field values that define this aggregation group. Keys are the groupBy field names, values are the field values for this group.\",\n            \"example\": {}\n          },\n          \"count\": {\n            \"type\": \"integer\",\n            \"description\": \"The number of log records in this aggregation group.\",\n            \"format\": \"int64\",\n            \"example\"\
  : 500\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogAggregateResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-log-monitoring-v2-log-aggregate-result-schema.json
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
