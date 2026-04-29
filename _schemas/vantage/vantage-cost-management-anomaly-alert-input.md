---
description: ''
layout: schema
name: AnomalyAlertInput
properties_list:
- description: The token of the Cost Report to monitor.
  name: cost_report_token
  type: string
- description: The threshold percentage for anomaly detection.
  name: threshold
  type: number
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-anomaly-alert-input-schema.json
slug: vantage-cost-management-anomaly-alert-input
source_filename: vantage-cost-management-anomaly-alert-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnomalyAlertInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cost_report_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Cost Report to monitor.\"\n    },\n    \"threshold\": {\n      \"type\": \"number\",\n      \"description\": \"The threshold percentage for anomaly detection.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-anomaly-alert-input-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: AnomalyAlertInput
---
