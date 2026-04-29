---
description: Export job details
layout: schema
name: ExportDetail
properties_list:
- description: Unique export identifier
  name: export_id
  type: string
- description: Export processing status
  name: status
  type: string
- description: Export file format
  name: format
  type: string
- description: Export creation timestamp
  name: created_at
  type: string
- description: Export completion timestamp
  name: completed_at
  type: string
- description: URL to download the exported file
  name: download_url
  type: string
- description: Size of the exported file in bytes
  name: file_size_bytes
  type: integer
provider_name: Circana
provider_slug: circana
schema_file: json-schema/liquid-data-export-detail-schema.json
slug: liquid-data-export-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-export-detail-schema.json\",\n  \"title\": \"ExportDetail\",\n  \"description\": \"Export job details\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"export_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique export identifier\",\n      \"example\": \"exp-500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Export processing status\",\n      \"enum\": [\"processing\", \"completed\", \"failed\"],\n      \"example\": \"completed\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"Export file format\",\n      \"example\": \"csv\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Export creation timestamp\",\n      \"example\": \"2026-04-18T12:00:00Z\"\
  \n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Export completion timestamp\",\n      \"example\": \"2026-04-18T12:02:00Z\"\n    },\n    \"download_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the exported file\",\n      \"example\": \"https://exports.circana.com/exp-500123/data.csv\"\n    },\n    \"file_size_bytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the exported file in bytes\",\n      \"example\": 2456789\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-export-detail-schema.json
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
title: ExportDetail
---
