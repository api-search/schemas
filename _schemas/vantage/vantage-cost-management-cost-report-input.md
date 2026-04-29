---
description: ''
layout: schema
name: CostReportInput
properties_list:
- description: The title of the Cost Report.
  name: title
  type: string
- description: VQL filter expression for the Cost Report.
  name: filter
  type: string
- description: Groupings for the Cost Report.
  name: groupings
  type: string
- description: The token of the Folder to place the report in.
  name: folder_token
  type: string
- description: Tokens of Saved Filters to apply.
  name: saved_filter_tokens
  type: array
- description: The token of the Workspace for the report.
  name: workspace_token
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-cost-report-input-schema.json
slug: vantage-cost-management-cost-report-input
source_filename: vantage-cost-management-cost-report-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CostReportInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Cost Report.\"\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"VQL filter expression for the Cost Report.\"\n    },\n    \"groupings\": {\n      \"type\": \"string\",\n      \"description\": \"Groupings for the Cost Report.\"\n    },\n    \"folder_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Folder to place the report in.\"\n    },\n    \"saved_filter_tokens\": {\n      \"type\": \"array\",\n      \"description\": \"Tokens of Saved Filters to apply.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace for the report.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-cost-report-input-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: CostReportInput
---
