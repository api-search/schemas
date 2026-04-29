---
description: Response containing the generated report details.
layout: schema
name: Report Response
properties_list:
- description: Unique identifier for the generated report.
  name: reportId
  type: string
- description: Current status of the report generation.
  name: status
  type: string
- description: Timestamp when the report was created.
  name: createdAt
  type: string
- description: URL to download the completed report.
  name: downloadUrl
  type: string
provider_name: albertsons
provider_slug: albertsons
schema_file: json-schema/retail-media-api-report-response-schema.json
slug: retail-media-api-report-response
source_filename: retail-media-api-report-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-report-response-schema.json\",\n  \"title\": \"Report Response\",\n  \"description\": \"Response containing the generated report details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the generated report.\",\n      \"example\": \"rpt-abc123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"completed\",\n        \"failed\"\n      ],\n      \"description\": \"Current status of the report generation.\",\n      \"example\": \"completed\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the report was created.\",\n      \"example\"\
  : \"2026-04-19T10:30:00Z\"\n    },\n    \"downloadUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to download the completed report.\",\n      \"example\": \"https://api.albertsons.com/reports/rpt-abc123/download\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-report-response-schema.json
tags:
- Grocery
- Retail
- Retail Media
- Advertising
- Campaigns
- Analytics
- Consumer Goods
- Food
- Pharmacy
title: Report Response
---
