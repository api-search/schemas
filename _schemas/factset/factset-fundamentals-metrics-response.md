---
description: Response wrapper containing an array of available metrics and their metadata.
layout: schema
name: MetricsResponse
properties_list:
- description: Array of metric objects representing the metrics that can be requested from the fundamentals APIs.
  name: data
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-metrics-response-schema.json
slug: factset-fundamentals-metrics-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricsResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response wrapper containing an array of available metrics and their metadata.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of metric objects representing the metrics that can be requested from the fundamentals APIs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-metrics-response-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: MetricsResponse
---
