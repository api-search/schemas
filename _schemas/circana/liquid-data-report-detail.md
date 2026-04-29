---
description: Detailed report information
layout: schema
name: ReportDetail
properties_list:
- description: Unique report identifier
  name: report_id
  type: string
- description: Report name
  name: name
  type: string
- description: Report processing status
  name: status
  type: string
- description: Report creation timestamp
  name: created_at
  type: string
- description: Report completion timestamp
  name: completed_at
  type: string
- description: Primary category for the report
  name: category
  type: string
- description: Type of report
  name: report_type
  type: string
- description: Number of data rows in completed report
  name: row_count
  type: integer
- description: Estimated completion time for processing reports
  name: estimated_completion
  type: string
provider_name: Circana
provider_slug: circana
schema_file: json-schema/liquid-data-report-detail-schema.json
slug: liquid-data-report-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-report-detail-schema.json\",\n  \"title\": \"ReportDetail\",\n  \"description\": \"Detailed report information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"report_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique report identifier\",\n      \"example\": \"rpt-500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Report name\",\n      \"example\": \"Q1 2026 Beverage Market Review\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Report processing status\",\n      \"enum\": [\"draft\", \"processing\", \"completed\", \"failed\"],\n      \"example\": \"completed\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Report creation timestamp\"\
  ,\n      \"example\": \"2026-04-01T10:00:00Z\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Report completion timestamp\",\n      \"example\": \"2026-04-01T10:03:00Z\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Primary category for the report\",\n      \"example\": \"Beverages\"\n    },\n    \"report_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of report\",\n      \"example\": \"market_review\"\n    },\n    \"row_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of data rows in completed report\",\n      \"example\": 4523\n    },\n    \"estimated_completion\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Estimated completion time for processing reports\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-report-detail-schema.json
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
title: ReportDetail
---
