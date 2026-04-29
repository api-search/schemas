---
description: A Business Metric that tracks custom business values over time and can be associated with Cost Reports for unit economics.
layout: schema
name: Vantage Business Metric
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
schema_file: json-schema/business-metric.json
slug: business-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/business-metric.json\",\n  \"title\": \"Vantage Business Metric\",\n  \"description\": \"A Business Metric that tracks custom business values over time and can be associated with Cost Reports for unit economics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Business Metric.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Business Metric.\"\n    },\n    \"cost_report_tokens_with_metadata\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Associated cost reports with metadata.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\"\
  : {\n          \"date\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          },\n          \"amount\": {\n            \"type\": \"number\"\n          }\n        }\n      },\n      \"description\": \"The values of the Business Metric over time.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the Business Metric was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/business-metric.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Business Metric
---
