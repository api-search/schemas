---
description: ReportRequest schema from ARGUS Enterprise API
layout: schema
name: ReportRequest
properties_list:
- description: ''
  name: reportType
  type: string
- description: ''
  name: title
  type: string
- description: Properties to include in the report
  name: propertyIds
  type: array
- description: Portfolios to include in the report
  name: portfolioIds
  type: array
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: outputFormat
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-report-request-schema.json
slug: argus-enterprise-report-request
source_filename: argus-enterprise-report-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-report-request-schema.json\",\n  \"title\": \"ReportRequest\",\n  \"description\": \"ReportRequest schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PropertySummary\",\n        \"PortfolioSummary\",\n        \"CashFlowAnalysis\",\n        \"ValuationSummary\",\n        \"LeaseExpiry\",\n        \"TenantRoll\",\n        \"CapitalExpenditure\"\n      ]\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"propertyIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      },\n      \"description\": \"Properties to include in the report\"\n    },\n    \"portfolioIds\": {\n      \"type\": \"array\"\
  ,\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      },\n      \"description\": \"Portfolios to include in the report\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"outputFormat\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PDF\",\n        \"Excel\",\n        \"CSV\"\n      ],\n      \"default\": \"PDF\"\n    }\n  },\n  \"required\": [\n    \"reportType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-report-request-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: ReportRequest
---
