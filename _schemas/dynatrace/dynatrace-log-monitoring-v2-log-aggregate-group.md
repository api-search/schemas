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
schema_file: json-schema/dynatrace-log-monitoring-v2-log-aggregate-group-schema.json
slug: dynatrace-log-monitoring-v2-log-aggregate-group
source_filename: dynatrace-log-monitoring-v2-log-aggregate-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A single aggregation group result.\",\n  \"properties\": {\n    \"groupByFields\": {\n      \"type\": \"object\",\n      \"description\": \"The field values that define this aggregation group. Keys are the groupBy field names, values are the field values for this group.\",\n      \"example\": {}\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of log records in this aggregation group.\",\n      \"format\": \"int64\",\n      \"example\": 500\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogAggregateGroup\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-log-monitoring-v2-log-aggregate-group-schema.json
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
