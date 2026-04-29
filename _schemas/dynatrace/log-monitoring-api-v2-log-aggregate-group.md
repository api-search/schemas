---
description: A single aggregation group result.
layout: schema
name: LogAggregateGroup
properties_list:
- description: The field values that define this aggregation group. Keys are the groupBy field names, values are the field values for this group.
  name: groupByFields
  type: object
- description: The number of log records in this aggregation group.
  name: count
  type: integer
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/log-monitoring-api-v2-log-aggregate-group-schema.json
slug: log-monitoring-api-v2-log-aggregate-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/log-monitoring-api-v2-log-aggregate-group-schema.json\",\n  \"title\": \"LogAggregateGroup\",\n  \"description\": \"A single aggregation group result.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groupByFields\": {\n      \"type\": \"object\",\n      \"description\": \"The field values that define this aggregation group. Keys are the groupBy field names, values are the field values for this group.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {}\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The number of log records in this aggregation group.\",\n      \"example\": 500\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/log-monitoring-api-v2-log-aggregate-group-schema.json
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
title: LogAggregateGroup
---
