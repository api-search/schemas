---
description: Request body for generating a custom performance report.
layout: schema
name: Report Request
properties_list:
- description: List of campaign IDs to include in the report. Empty returns all.
  name: campaignIds
  type: array
- description: Start date for the report period (ISO 8601).
  name: startDate
  type: string
- description: End date for the report period (ISO 8601).
  name: endDate
  type: string
- description: Dimensions to group report data by.
  name: dimensions
  type: array
- description: Metrics to include in the report.
  name: metrics
  type: array
- description: Output format for the report.
  name: format
  type: string
provider_name: albertsons
provider_slug: albertsons
schema_file: json-schema/retail-media-api-report-request-schema.json
slug: retail-media-api-report-request
source_filename: retail-media-api-report-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-report-request-schema.json\",\n  \"title\": \"Report Request\",\n  \"description\": \"Request body for generating a custom performance report.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"campaignIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of campaign IDs to include in the report. Empty returns all.\",\n      \"example\": [\n        \"500123\"\n      ]\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Start date for the report period (ISO 8601).\",\n      \"example\": \"2026-03-01\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"End date for the report period (ISO 8601).\"\
  ,\n      \"example\": \"2026-03-31\"\n    },\n    \"dimensions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Dimensions to group report data by.\",\n      \"example\": [\n        \"date\",\n        \"campaign\"\n      ]\n    },\n    \"metrics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Metrics to include in the report.\",\n      \"example\": [\n        \"impressions\",\n        \"clicks\",\n        \"roas\"\n      ]\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"json\",\n        \"csv\"\n      ],\n      \"description\": \"Output format for the report.\",\n      \"example\": \"json\"\n    }\n  },\n  \"required\": [\n    \"startDate\",\n    \"endDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/albertsons/refs/heads/main/json-schema/retail-media-api-report-request-schema.json
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
title: Report Request
---
