---
description: ''
layout: schema
name: FinancialCommitmentReportInput
properties_list:
- description: The title of the Financial Commitment Report.
  name: title
  type: string
- description: The token of the Workspace for the report.
  name: workspace_token
  type: string
provider_name: Vantage
provider_slug: vantage
schema_file: json-schema/vantage-cost-management-financial-commitment-report-input-schema.json
slug: vantage-cost-management-financial-commitment-report-input
source_filename: vantage-cost-management-financial-commitment-report-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FinancialCommitmentReportInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the Financial Commitment Report.\"\n    },\n    \"workspace_token\": {\n      \"type\": \"string\",\n      \"description\": \"The token of the Workspace for the report.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/json-schema/vantage-cost-management-financial-commitment-report-input-schema.json
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
title: FinancialCommitmentReportInput
---
