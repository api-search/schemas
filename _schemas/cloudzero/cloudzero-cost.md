---
description: Represents a cost data record returned by the CloudZero Billing API, including grouped dimensions and time-series cost values.
layout: schema
name: CloudZero Cost
properties_list:
- description: Key-value pairs representing the dimensions this cost record is grouped by (e.g., Account, Service, Region).
  name: group
  type: object
- description: Time-series array of cost data points.
  name: cost
  type: array
provider_name: CloudZero
provider_slug: cloudzero
schema_file: json-schema/cloudzero-cost.json
slug: cloudzero-cost
source_filename: cloudzero-cost.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cloudzero/blob/main/json-schema/cloudzero-cost.json\",\n  \"title\": \"CloudZero Cost\",\n  \"description\": \"Represents a cost data record returned by the CloudZero Billing API, including grouped dimensions and time-series cost values.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs representing the dimensions this cost record is grouped by (e.g., Account, Service, Region).\"\n    },\n    \"cost\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"timestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Timestamp for the cost data point.\"\n          },\n       \
  \   \"value\": {\n            \"type\": \"number\",\n            \"format\": \"double\",\n            \"description\": \"Cost amount for the data point.\"\n          }\n        },\n        \"required\": [\n          \"timestamp\",\n          \"value\"\n        ]\n      },\n      \"description\": \"Time-series array of cost data points.\"\n    }\n  },\n  \"required\": [\n    \"group\",\n    \"cost\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/json-schema/cloudzero-cost.json
tags:
- Budgets
- Cloud Cost Management
- Cost Allocation
- Cost Optimization
- FinOps
- Telemetry
- Unit Economics
title: CloudZero Cost
---
