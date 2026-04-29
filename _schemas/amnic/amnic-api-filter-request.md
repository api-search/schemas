---
description: Request body for retrieving chart data with additional custom filters.
layout: schema
name: FilterRequest
properties_list:
- description: Additional filters to apply when retrieving chart data.
  name: filters
  type: array
provider_name: Amnic
provider_slug: amnic
schema_file: json-schema/amnic-api-filter-request-schema.json
slug: amnic-api-filter-request
source_filename: amnic-api-filter-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amnic/refs/heads/main/json-schema/amnic-api-filter-request-schema.json\",\n  \"title\": \"FilterRequest\",\n  \"description\": \"Request body for retrieving chart data with additional custom filters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"type\": \"array\",\n      \"description\": \"Additional filters to apply when retrieving chart data.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Filter\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amnic/refs/heads/main/json-schema/amnic-api-filter-request-schema.json
tags:
- Cloud Cost Observability
- FinOps
- Cloud Cost Management
- Cost Optimization
- Kubernetes
- AWS
- Azure
- Google Cloud
title: FilterRequest
---
