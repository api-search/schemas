---
description: A group-by configuration for aggregating log results by facet values
layout: schema
name: LogsGroupBy
properties_list:
- description: The log attribute or tag to group results by
  name: facet
  type: string
- description: The maximum number of unique facet values to return in results
  name: limit
  type: integer
- description: Sort configuration for group-by results
  name: sort
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-logs-logs-group-by-schema.json
slug: datadog-logs-logs-group-by
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-group-by-schema.json\",\n  \"title\": \"LogsGroupBy\",\n  \"description\": \"A group-by configuration for aggregating log results by facet values\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"facet\": {\n      \"type\": \"string\",\n      \"description\": \"The log attribute or tag to group results by\",\n      \"example\": \"example_value\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of unique facet values to return in results\",\n      \"default\": 10,\n      \"example\": 42\n    },\n    \"sort\": {\n      \"type\": \"object\",\n      \"description\": \"Sort configuration for group-by results\",\n      \"properties\": {\n        \"aggregation\": {\n          \"type\": \"string\",\n          \"description\": \"The aggregation\
  \ metric to sort by\",\n          \"enum\": [\n            \"count\",\n            \"cardinality\",\n            \"pc75\",\n            \"pc90\",\n            \"pc95\",\n            \"pc98\",\n            \"pc99\",\n            \"sum\",\n            \"avg\",\n            \"min\",\n            \"max\"\n          ]\n        },\n        \"order\": {\n          \"type\": \"string\",\n          \"description\": \"The sort direction for group-by results\",\n          \"enum\": [\n            \"asc\",\n            \"desc\"\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"facet\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-group-by-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: LogsGroupBy
---
