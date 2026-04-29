---
description: The result of an analytics report request
layout: schema
name: ReportResponse
properties_list:
- description: Total number of result pages
  name: totalPages
  type: integer
- description: Number of rows in this response
  name: numberOfElements
  type: integer
- description: ''
  name: rows
  type: array
- description: Column metadata for the report
  name: columns
  type: object
- description: Totals and summary statistics
  name: summaryData
  type: object
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-report-response-schema.json
slug: adobe-analytics-report-response
source_filename: adobe-analytics-report-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result of an analytics report request\",\n  \"properties\": {\n    \"totalPages\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of result pages\",\n      \"example\": 42\n    },\n    \"numberOfElements\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows in this response\",\n      \"example\": 10\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single row in a report result\",\n        \"properties\": {\n          \"itemId\": {\n            \"type\": \"string\",\n            \"description\": \"The dimension item ID\",\n            \"example\": \"500123\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"The dimension item display value\",\n            \"example\": \"example_value\"\n          },\n          \"data\"\
  : {\n            \"type\": \"array\",\n            \"description\": \"Metric values for this row, in column order\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"number\"\n            }\n          }\n        }\n      }\n    },\n    \"columns\": {\n      \"type\": \"object\",\n      \"description\": \"Column metadata for the report\",\n      \"example\": \"example_value\"\n    },\n    \"summaryData\": {\n      \"type\": \"object\",\n      \"description\": \"Totals and summary statistics\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-report-response-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ReportResponse
---
