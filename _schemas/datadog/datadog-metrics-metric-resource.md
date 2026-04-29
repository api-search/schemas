---
description: A resource (such as a host or service) associated with a metric series
layout: schema
name: MetricResource
properties_list:
- description: The name of the resource (e.g., hostname or service name)
  name: name
  type: string
- description: The type of the resource (e.g., host, service, container)
  name: type
  type: string
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-metrics-metric-resource-schema.json
slug: datadog-metrics-metric-resource
source_filename: datadog-metrics-metric-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-resource-schema.json\",\n  \"title\": \"MetricResource\",\n  \"description\": \"A resource (such as a host or service) associated with a metric series\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource (e.g., hostname or service name)\",\n      \"example\": \"Example Monitor\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource (e.g., host, service, container)\",\n      \"example\": \"metric alert\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-resource-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MetricResource
---
