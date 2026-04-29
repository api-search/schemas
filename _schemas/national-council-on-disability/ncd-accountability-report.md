---
description: Annual performance and accountability report from the National Council on Disability.
layout: schema
name: NCD Accountability Report
properties_list:
- description: Type of accountability report
  name: reportType
  type: string
- description: Fiscal year covered by the report
  name: fiscalYear
  type: string
- description: Full report title
  name: title
  type: string
- description: Total agency budget in dollars for the fiscal year
  name: agencyBudget
  type: number
- description: List of performance goals for the period
  name: performanceGoals
  type: array
- description: Results achieved against performance goals
  name: performanceResults
  type: array
- description: URL to download the full report
  name: documentURL
  type: string
- description: Date the report was published
  name: publishedDate
  type: string
provider_name: National Council on Disability
provider_slug: national-council-on-disability
schema_file: json-schema/ncd-accountability-report-schema.json
slug: ncd-accountability-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.ncd.gov/schemas/accountability-report\",\n  \"title\": \"NCD Accountability Report\",\n  \"description\": \"Annual performance and accountability report from the National Council on Disability.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"reportType\",\n    \"fiscalYear\"\n  ],\n  \"properties\": {\n    \"reportType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AnnualPerformanceReport\",\n        \"CongressionalBudgetJustification\",\n        \"FinancialAudit\",\n        \"StrategicPlan\"\n      ],\n      \"description\": \"Type of accountability report\"\n    },\n    \"fiscalYear\": {\n      \"type\": \"string\",\n      \"description\": \"Fiscal year covered by the report\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Full report title\"\n    },\n    \"agencyBudget\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Total agency budget in dollars for the fiscal year\"\n    },\n    \"performanceGoals\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of performance goals for the period\"\n    },\n    \"performanceResults\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Results achieved against performance goals\"\n    },\n    \"documentURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the full report\"\n    },\n    \"publishedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the report was published\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/national-council-on-disability/refs/heads/main/json-schema/ncd-accountability-report-schema.json
tags:
- Disability
- Federal Government
- Policy
- Civil Rights
- Healthcare
- Independent Agency
title: NCD Accountability Report
---
