---
description: Represents a telemetry record for sending unit metric or allocation data to CloudZero for cost analysis and unit economics calculations.
layout: schema
name: CloudZero Telemetry Record
properties_list:
- description: Timestamp for the telemetry record.
  name: timestamp
  type: string
- description: Numeric value for the metric or allocation.
  name: value
  type: number
- description: Time granularity of the record.
  name: granularity
  type: string
- description: Key-value pairs for filtering and grouping unit metric telemetry.
  name: filter
  type: object
- description: Key-value pairs identifying the element being allocated for allocation telemetry.
  name: element
  type: object
provider_name: CloudZero
provider_slug: cloudzero
schema_file: json-schema/cloudzero-telemetry-record.json
slug: cloudzero-telemetry-record
source_filename: cloudzero-telemetry-record.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cloudzero/blob/main/json-schema/cloudzero-telemetry-record.json\",\n  \"title\": \"CloudZero Telemetry Record\",\n  \"description\": \"Represents a telemetry record for sending unit metric or allocation data to CloudZero for cost analysis and unit economics calculations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp for the telemetry record.\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Numeric value for the metric or allocation.\"\n    },\n    \"granularity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HOURLY\",\n        \"DAILY\",\n        \"MONTHLY\"\n      ],\n      \"description\": \"Time granularity of the record.\"\n    },\n    \"filter\": {\n   \
  \   \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for filtering and grouping unit metric telemetry.\"\n    },\n    \"element\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs identifying the element being allocated for allocation telemetry.\"\n    }\n  },\n  \"required\": [\n    \"timestamp\",\n    \"value\",\n    \"granularity\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/json-schema/cloudzero-telemetry-record.json
tags:
- Budgets
- Cloud Cost Management
- Cost Allocation
- Cost Optimization
- FinOps
- Telemetry
- Unit Economics
title: CloudZero Telemetry Record
---
