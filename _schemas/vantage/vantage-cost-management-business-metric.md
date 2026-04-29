---
description: ''
layout: schema
name: BusinessMetric
properties_list:
- description: The unique token identifier for the Business Metric.
  name: token
  type: string
- description: The title of the Business Metric.
  name: title
  type: string
- description: Associated cost reports with metadata.
  name: cost_report_tokens_with_metadata
  type: array
- description: The values of the Business Metric over time.
  name: values
  type: array
- description: The date and time the Business Metric was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-business-metric-schema.json
slug: vantage-cost-management-business-metric
source_filename: vantage-cost-management-business-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BusinessMetric\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Business Metric.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Business Metric.\"\n    },\n    \"cost_report_tokens_with_metadata\": {\n      \"type\": \"array\",\n      \"description\": \"Associated cost reports with metadata.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"The values of the Business Metric over time.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the Business Metric was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-business-metric-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: BusinessMetric
---
