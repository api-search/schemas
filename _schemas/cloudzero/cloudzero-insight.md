---
description: Represents a cost insight for tracking cost anomalies and patterns within CloudZero.
layout: schema
name: CloudZero Insight
properties_list:
- description: Unique identifier for the insight.
  name: id
  type: string
- description: Display name for the insight.
  name: name
  type: string
- description: Description of what the insight tracks.
  name: description
  type: string
- description: Timestamp when the insight was created.
  name: created_at
  type: string
- description: Timestamp when the insight was last updated.
  name: updated_at
  type: string
- description: Filters applied to the insight for narrowing cost data.
  name: filters
  type: object
- description: Dimensions used for grouping cost data within the insight.
  name: group_by
  type: array
provider_name: CloudZero
provider_slug: cloudzero
schema_file: json-schema/cloudzero-insight.json
slug: cloudzero-insight
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/cloudzero/blob/main/json-schema/cloudzero-insight.json\",\n  \"title\": \"CloudZero Insight\",\n  \"description\": \"Represents a cost insight for tracking cost anomalies and patterns within CloudZero.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the insight.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the insight.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the insight tracks.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the insight was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Timestamp when the insight was last updated.\"\n    },\n    \"filters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Filters applied to the insight for narrowing cost data.\"\n    },\n    \"group_by\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Dimensions used for grouping cost data within the insight.\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudzero/refs/heads/main/json-schema/cloudzero-insight.json
tags:
- Budgets
- Cloud Cost Management
- Cost Allocation
- Cost Optimization
- FinOps
- Telemetry
- Unit Economics
title: CloudZero Insight
---
