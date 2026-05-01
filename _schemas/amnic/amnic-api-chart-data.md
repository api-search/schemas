---
description: Cost chart data returned as a 2D array with headers and rows.
layout: schema
name: ChartData
properties_list:
- description: Column headers for the cost data result set.
  name: headers
  type: array
- description: Rows of cost data values corresponding to the headers.
  name: rows
  type: array
provider_name: Amnic
provider_slug: amnic
schema_file: json-schema/amnic-api-chart-data-schema.json
slug: amnic-api-chart-data
source_filename: amnic-api-chart-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amnic/refs/heads/main/json-schema/amnic-api-chart-data-schema.json\",\n  \"title\": \"ChartData\",\n  \"description\": \"Cost chart data returned as a 2D array with headers and rows.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"headers\": {\n      \"type\": \"array\",\n      \"description\": \"Column headers for the cost data result set.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"date\",\n        \"service\",\n        \"cost\"\n      ]\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"description\": \"Rows of cost data values corresponding to the headers.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amnic/refs/heads/main/json-schema/amnic-api-chart-data-schema.json
tags:
- Cloud Cost Observability
- FinOps
- Cloud Cost Management
- Cost Optimization
- Kubernetes
- Azure
- Google Cloud
title: ChartData
---
