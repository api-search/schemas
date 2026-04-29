---
description: ''
layout: schema
name: SegmentInput
properties_list:
- description: The title of the Segment.
  name: title
  type: string
- description: The VQL filter expression.
  name: filter
  type: string
- description: The priority order of the Segment.
  name: priority
  type: integer
- description: The token of the Workspace for the Segment.
  name: workspace_token
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-segment-input-schema.json
slug: vantage-cost-management-segment-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SegmentInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Segment.\"\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"The VQL filter expression.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"The priority order of the Segment.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace for the Segment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-segment-input-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: SegmentInput
---
