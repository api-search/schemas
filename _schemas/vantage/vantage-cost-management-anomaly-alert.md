---
description: ''
layout: schema
name: AnomalyAlert
properties_list:
- description: The unique token identifier for the Anomaly Alert.
  name: token
  type: string
- description: The token of the associated Cost Report.
  name: cost_report_token
  type: string
- description: The threshold percentage for anomaly detection.
  name: threshold
  type: number
- description: The date and time the Anomaly Alert was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-anomaly-alert-schema.json
slug: vantage-cost-management-anomaly-alert
source_filename: vantage-cost-management-anomaly-alert-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnomalyAlert\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Anomaly Alert.\"\n    },\n    \"cost_report_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the associated Cost Report.\"\n    },\n    \"threshold\": {\n      \"type\": \"number\",\n      \"description\": \"The threshold percentage for anomaly detection.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the Anomaly Alert was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-anomaly-alert-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: AnomalyAlert
---
