---
description: Represents cost data in CloudZero Common Bill Format (CBF) for ingestion via the AnyCost Stream Adaptor.
layout: schema
name: CloudZero Billing Drop
properties_list:
- description: Array of cost line items in Common Bill Format.
  name: line_items
  type: array
provider_name: CloudZero
provider_slug: cloudzero
schema_file: json-schema/cloudzero-billing-drop.json
slug: cloudzero-billing-drop
source_filename: cloudzero-billing-drop.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cloudzero/blob/main/json-schema/cloudzero-billing-drop.json\",\n  \"title\": \"CloudZero Billing Drop\",\n  \"description\": \"Represents cost data in CloudZero Common Bill Format (CBF) for ingestion via the AnyCost Stream Adaptor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"line_items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"timestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Timestamp for the billing line item.\"\n          },\n          \"cost\": {\n            \"type\": \"number\",\n            \"format\": \"double\",\n            \"description\": \"Cost amount for the line item.\"\n          },\n          \"service\": {\n            \"type\": \"string\",\n            \"description\": \"Service\
  \ name associated with the cost.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"Description of the cost line item.\"\n          },\n          \"metadata\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Additional metadata key-value pairs for the line item.\"\n          }\n        },\n        \"required\": [\n          \"timestamp\",\n          \"cost\"\n        ]\n      },\n      \"description\": \"Array of cost line items in Common Bill Format.\"\n    }\n  },\n  \"required\": [\n    \"line_items\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/json-schema/cloudzero-billing-drop.json
tags:
- Budgets
- Cloud Cost Management
- Cost Allocation
- Cost Optimization
- FinOps
- Telemetry
- Unit Economics
title: CloudZero Billing Drop
---
