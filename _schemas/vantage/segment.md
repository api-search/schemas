---
description: A Segment for allocating cloud costs using VQL filters with priority-based ordering.
layout: schema
name: Vantage Segment
properties_list:
- description: The unique token identifier for the Segment.
  name: token
  type: string
- description: The title of the Segment.
  name: title
  type: string
- description: The VQL filter expression for the Segment.
  name: filter
  type: string
- description: The priority order of the Segment.
  name: priority
  type: integer
- description: The token of the Workspace this Segment belongs to.
  name: workspace_token
  type: string
- description: The date and time the Segment was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/segment.json
slug: segment
source_filename: segment.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/vantage/blob/main/json-schema/segment.json\",\n  \"title\": \"Vantage Segment\",\n  \"description\": \"A Segment for allocating cloud costs using VQL filters with priority-based ordering.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Segment.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Segment.\"\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"The VQL filter expression for the Segment.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"The priority order of the Segment.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace this Segment belongs to.\"\n    },\n  \
  \  \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the Segment was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/segment.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: Vantage Segment
---
