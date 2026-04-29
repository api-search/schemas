---
description: ''
layout: schema
name: ResourceReport
properties_list:
- description: The unique token identifier for the Resource Report.
  name: token
  type: string
- description: The title of the Resource Report.
  name: title
  type: string
- description: The VQL filter applied to the Resource Report.
  name: filter
  type: string
- description: The token of the Workspace this report belongs to.
  name: workspace_token
  type: string
- description: The date and time the Resource Report was created.
  name: created_at
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-resource-report-schema.json
slug: vantage-cost-management-resource-report
source_filename: vantage-cost-management-resource-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourceReport\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The unique token identifier for the Resource Report.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Resource Report.\"\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"The VQL filter applied to the Resource Report.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace this report belongs to.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the Resource Report was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-resource-report-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: ResourceReport
---
