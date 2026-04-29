---
description: ''
layout: schema
name: BusinessMetricInput
properties_list:
- description: The title of the Business Metric.
  name: title
  type: string
- description: The values of the Business Metric.
  name: values
  type: array
- description: Associated cost reports with metadata.
  name: cost_report_tokens_with_metadata
  type: array
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-business-metric-input-schema.json
slug: vantage-cost-management-business-metric-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BusinessMetricInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Business Metric.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"The values of the Business Metric.\"\n    },\n    \"cost_report_tokens_with_metadata\": {\n      \"type\": \"array\",\n      \"description\": \"Associated cost reports with metadata.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-business-metric-input-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: BusinessMetricInput
---
