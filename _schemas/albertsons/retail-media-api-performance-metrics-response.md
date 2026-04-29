---
description: Collection of performance metric data points.
layout: schema
name: Performance Metrics Response
properties_list:
- description: Array of performance metric data points.
  name: metrics
  type: array
- description: Total number of metric records returned.
  name: total
  type: integer
provider_name: albertsons
provider_slug: albertsons
schema_file: json-schema/retail-media-api-performance-metrics-response-schema.json
slug: retail-media-api-performance-metrics-response
source_filename: retail-media-api-performance-metrics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-performance-metrics-response-schema.json\",\n  \"title\": \"Performance Metrics Response\",\n  \"description\": \"Collection of performance metric data points.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metrics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PerformanceMetric\"\n      },\n      \"description\": \"Array of performance metric data points.\"\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of metric records returned.\",\n      \"example\": 31\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-performance-metrics-response-schema.json
tags:
- Grocery
- Retail
- Retail Media
- Advertising
- Campaigns
- Analytics
- Consumer Goods
- Food
- Pharmacy
title: Performance Metrics Response
---
