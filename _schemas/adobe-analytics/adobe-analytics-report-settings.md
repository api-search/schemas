---
description: Settings that control report output behavior
layout: schema
name: ReportSettings
properties_list:
- description: Maximum number of rows to return
  name: limit
  type: integer
- description: Page number (zero-indexed)
  name: page
  type: integer
- description: How to handle None values
  name: nonesBehavior
  type: string
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-report-settings-schema.json
slug: adobe-analytics-report-settings
source_filename: adobe-analytics-report-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Settings that control report output behavior\",\n  \"properties\": {\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of rows to return\",\n      \"example\": 10\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Page number (zero-indexed)\",\n      \"example\": 10\n    },\n    \"nonesBehavior\": {\n      \"type\": \"string\",\n      \"description\": \"How to handle None values\",\n      \"example\": \"exclude-nones\",\n      \"enum\": [\n        \"exclude-nones\",\n        \"return-nones\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportSettings\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-report-settings-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: ReportSettings
---
