---
description: An Anomaly Alert that monitors a Cost Report for unexpected cost spikes based on a percentage threshold.
layout: schema
name: Vantage Anomaly Alert
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
schema_file: json-schema/anomaly-alert.json
slug: anomaly-alert
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/anomaly-alert.json\",\n  \"title\": \"Vantage Anomaly Alert\",\n  \"description\": \"An Anomaly Alert that monitors a Cost Report for unexpected cost spikes based on a percentage threshold.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Anomaly Alert.\"\n    },\n    \"cost_report_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the associated Cost Report.\"\n    },\n    \"threshold\": {\n      \"type\": \"number\",\n      \"description\": \"The threshold percentage for anomaly detection.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the Anomaly Alert was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/anomaly-alert.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Anomaly Alert
---
