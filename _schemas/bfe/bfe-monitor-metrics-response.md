---
description: Metrics data for a specific monitor category.
layout: schema
name: MonitorMetricsResponse
properties_list:
- description: Name of the monitor category.
  name: name
  type: string
- description: Key-value pairs of metric names and values.
  name: metrics
  type: object
provider_name: BFE
provider_slug: bfe
schema_file: json-schema/bfe-monitor-metrics-response-schema.json
slug: bfe-monitor-metrics-response
source_filename: bfe-monitor-metrics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/json-schema/bfe-monitor-metrics-response-schema.json\",\n  \"title\": \"MonitorMetricsResponse\",\n  \"description\": \"Metrics data for a specific monitor category.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the monitor category.\",\n      \"example\": \"connections\"\n    },\n    \"metrics\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs of metric names and values.\",\n      \"additionalProperties\": {\n        \"type\": \"number\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/json-schema/bfe-monitor-metrics-response-schema.json
tags:
- Load Balancer
- Networking
- Open Source
- Traffic Management
- CNCF
- Baidu
title: MonitorMetricsResponse
---
