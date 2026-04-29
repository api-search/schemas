---
description: A single row in a report result
layout: schema
name: ReportRow
properties_list:
- description: The dimension item ID
  name: itemId
  type: string
- description: The dimension item display value
  name: value
  type: string
- description: Metric values for this row, in column order
  name: data
  type: array
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-report-row-schema.json
slug: adobe-analytics-report-row
source_filename: adobe-analytics-report-row-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A single row in a report result\",\n  \"properties\": {\n    \"itemId\": {\n      \"type\": \"string\",\n      \"description\": \"The dimension item ID\",\n      \"example\": \"500123\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The dimension item display value\",\n      \"example\": \"example_value\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Metric values for this row, in column order\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"number\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportRow\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-report-row-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ReportRow
---
