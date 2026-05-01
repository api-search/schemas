---
description: A filter object specifying a dimension and its accepted values for cost data queries.
layout: schema
name: Filter
properties_list:
- description: The dimension to filter by (e.g., service, region, account, team).
  name: filter_by
  type: string
- description: The list of values to include for the specified filter dimension.
  name: values
  type: array
provider_name: Amnic
provider_slug: amnic
schema_file: json-schema/amnic-api-filter-schema.json
slug: amnic-api-filter
source_filename: amnic-api-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amnic/refs/heads/main/json-schema/amnic-api-filter-schema.json\",\n  \"title\": \"Filter\",\n  \"description\": \"A filter object specifying a dimension and its accepted values for cost data queries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter_by\": {\n      \"type\": \"string\",\n      \"description\": \"The dimension to filter by (e.g., service, region, account, team).\",\n      \"example\": \"service\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"The list of values to include for the specified filter dimension.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"EC2\",\n        \"S3\"\n      ]\n    }\n  },\n  \"required\": [\n    \"filter_by\",\n    \"values\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amnic/refs/heads/main/json-schema/amnic-api-filter-schema.json
tags:
- Cloud Cost Observability
- FinOps
- Cloud Cost Management
- Cost Optimization
- Kubernetes
- Azure
- Google Cloud
title: Filter
---
