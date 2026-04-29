---
description: A metric query definition referencing a Datadog metrics query expression
layout: schema
name: MetricQueryDefinition
properties_list:
- description: A unique name used to reference this query in formula expressions
  name: name
  type: string
- description: The data source for the query
  name: data_source
  type: string
- description: The Datadog metrics query string (e.g., avg:system.cpu.user{*} by {host})
  name: query
  type: string
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-metrics-metric-query-definition-schema.json
slug: datadog-metrics-metric-query-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-query-definition-schema.json\",\n  \"title\": \"MetricQueryDefinition\",\n  \"description\": \"A metric query definition referencing a Datadog metrics query expression\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A unique name used to reference this query in formula expressions\",\n      \"example\": \"Example Monitor\"\n    },\n    \"data_source\": {\n      \"type\": \"string\",\n      \"description\": \"The data source for the query\",\n      \"enum\": [\n        \"metrics\",\n        \"cloud_cost\"\n      ],\n      \"example\": \"metrics\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The Datadog metrics query string (e.g., avg:system.cpu.user{*} by {host})\",\n      \"example\"\
  : \"avg:system.cpu.user{*}\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"data_source\",\n    \"query\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-query-definition-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MetricQueryDefinition
---
