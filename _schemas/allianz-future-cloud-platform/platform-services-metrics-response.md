---
description: Platform metrics for a service or overall platform
layout: schema
name: MetricsResponse
properties_list:
- description: Service the metrics apply to (null for platform-wide)
  name: service_id
  type: string
- description: Time range the metrics cover
  name: time_range_minutes
  type: integer
- description: Average CPU utilization percentage
  name: cpu_utilization
  type: number
- description: Average memory utilization percentage
  name: memory_utilization
  type: number
- description: Requests per minute
  name: request_rate
  type: number
- description: Error rate as a percentage
  name: error_rate
  type: number
- description: 99th percentile response latency in milliseconds
  name: p99_latency_ms
  type: integer
provider_name: Allianz Future Cloud Platform
provider_slug: allianz-future-cloud-platform
schema_file: json-schema/platform-services-metrics-response-schema.json
slug: platform-services-metrics-response
source_filename: platform-services-metrics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-metrics-response-schema.json\",\n  \"title\": \"MetricsResponse\",\n  \"description\": \"Platform metrics for a service or overall platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"service_id\": {\n      \"type\": \"string\",\n      \"description\": \"Service the metrics apply to (null for platform-wide)\",\n      \"example\": \"svc-500123\"\n    },\n    \"time_range_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Time range the metrics cover\",\n      \"example\": 60\n    },\n    \"cpu_utilization\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Average CPU utilization percentage\",\n      \"example\": 42.5\n    },\n    \"memory_utilization\": {\n      \"type\": \"number\",\n      \"format\":\
  \ \"double\",\n      \"description\": \"Average memory utilization percentage\",\n      \"example\": 68.2\n    },\n    \"request_rate\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Requests per minute\",\n      \"example\": 1250.0\n    },\n    \"error_rate\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Error rate as a percentage\",\n      \"example\": 0.12\n    },\n    \"p99_latency_ms\": {\n      \"type\": \"integer\",\n      \"description\": \"99th percentile response latency in milliseconds\",\n      \"example\": 145\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-future-cloud-platform/refs/heads/main/json-schema/platform-services-metrics-response-schema.json
tags:
- Cloud Platform
- Enterprise
- Financial Services
- Insurance
- Platform Engineering
- Kubernetes
title: MetricsResponse
---
