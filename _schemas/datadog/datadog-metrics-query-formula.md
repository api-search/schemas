---
description: A formula expression that combines one or more query results
layout: schema
name: QueryFormula
properties_list:
- description: The formula expression using query names as variables (e.g., query1 + query2)
  name: formula
  type: string
- description: An optional alias for the formula result used in the response
  name: alias
  type: string
- description: Optional limit configuration for top/bottom N results
  name: limit
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-metrics-query-formula-schema.json
slug: datadog-metrics-query-formula
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-query-formula-schema.json\",\n  \"title\": \"QueryFormula\",\n  \"description\": \"A formula expression that combines one or more query results\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"formula\": {\n      \"type\": \"string\",\n      \"description\": \"The formula expression using query names as variables (e.g., query1 + query2)\",\n      \"example\": \"example_value\"\n    },\n    \"alias\": {\n      \"type\": \"string\",\n      \"description\": \"An optional alias for the formula result used in the response\",\n      \"example\": \"example_value\"\n    },\n    \"limit\": {\n      \"type\": \"object\",\n      \"description\": \"Optional limit configuration for top/bottom N results\",\n      \"properties\": {\n        \"count\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"The number of results to return\"\n        },\n        \"order\": {\n          \"type\": \"string\",\n          \"description\": \"The sort order for limiting results\",\n          \"enum\": [\n            \"asc\",\n            \"desc\"\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"formula\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-query-formula-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: QueryFormula
---
