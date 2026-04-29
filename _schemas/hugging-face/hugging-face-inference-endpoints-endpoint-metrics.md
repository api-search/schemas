---
description: ''
layout: schema
name: EndpointMetrics
properties_list:
- description: ''
  name: request_count
  type: integer
- description: ''
  name: request_duration_ms
  type: object
- description: ''
  name: error_rate
  type: number
- description: ''
  name: tokens_per_second
  type: number
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-endpoints-endpoint-metrics-schema.json
slug: hugging-face-inference-endpoints-endpoint-metrics
source_filename: hugging-face-inference-endpoints-endpoint-metrics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EndpointMetrics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request_count\": {\n      \"type\": \"integer\"\n    },\n    \"request_duration_ms\": {\n      \"type\": \"object\"\n    },\n    \"error_rate\": {\n      \"type\": \"number\"\n    },\n    \"tokens_per_second\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-endpoints-endpoint-metrics-schema.json
tags: []
title: EndpointMetrics
---
