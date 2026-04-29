---
description: Report schema from ARGUS Enterprise API
layout: schema
name: Report
properties_list:
- description: Unique report identifier
  name: id
  type: string
- description: Type of report
  name: reportType
  type: string
- description: Report title
  name: title
  type: string
- description: Report generation status
  name: status
  type: string
- description: Report generation timestamp
  name: generatedAt
  type: string
- description: URL to download the completed report
  name: downloadUrl
  type: string
- description: Parameters used to generate the report
  name: parameters
  type: object
- description: Username of the report creator
  name: createdBy
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-report-schema.json
slug: argus-enterprise-report
source_filename: argus-enterprise-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-report-schema.json\",\n  \"title\": \"Report\",\n  \"description\": \"Report schema from ARGUS Enterprise API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique report identifier\"\n    },\n    \"reportType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PropertySummary\",\n        \"PortfolioSummary\",\n        \"CashFlowAnalysis\",\n        \"ValuationSummary\",\n        \"LeaseExpiry\",\n        \"TenantRoll\",\n        \"CapitalExpenditure\"\n      ],\n      \"description\": \"Type of report\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Report title\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n\
  \        \"Pending\",\n        \"Processing\",\n        \"Completed\",\n        \"Failed\"\n      ],\n      \"description\": \"Report generation status\"\n    },\n    \"generatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Report generation timestamp\"\n    },\n    \"downloadUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the completed report\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Parameters used to generate the report\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the report creator\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-report-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Report
---
