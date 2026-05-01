---
description: Represents a reporting request and its result in the DoorDash Reporting API, including report type, date range, processing status, and download information.
layout: schema
name: DoorDash Report
properties_list:
- description: The unique identifier for the report, assigned by DoorDash upon creation.
  name: report_id
  type: string
- description: The type of report to generate or that was generated.
  name: report_type
  type: string
- description: The start date for the report period in YYYY-MM-DD format.
  name: start_date
  type: string
- description: The end date for the report period in YYYY-MM-DD format.
  name: end_date
  type: string
- description: Optional list of store IDs to filter the report by specific stores.
  name: store_ids
  type: array
- description: The current processing status of the report.
  name: status
  type: string
- description: A temporary URL to download the completed report. Only present when status is SUCCEEDED.
  name: download_url
  type: string
- description: When the report request was created.
  name: created_at
  type: string
- description: When the report generation completed. Only present when status is SUCCEEDED or FAILED.
  name: completed_at
  type: string
provider_name: doordash
provider_slug: doordash
schema_file: json-schema/doordash-report-schema.json
slug: doordash-report
source_filename: doordash-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.doordash.com/schemas/doordash/report.json\",\n  \"title\": \"DoorDash Report\",\n  \"description\": \"Represents a reporting request and its result in the DoorDash Reporting API, including report type, date range, processing status, and download information.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"report_type\",\n    \"start_date\",\n    \"end_date\"\n  ],\n  \"properties\": {\n    \"report_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the report, assigned by DoorDash upon creation.\"\n    },\n    \"report_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of report to generate or that was generated.\",\n      \"enum\": [\n        \"financial\",\n        \"operations\",\n        \"menu\",\n        \"feedback\"\n      ]\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\":\
  \ \"date\",\n      \"description\": \"The start date for the report period in YYYY-MM-DD format.\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The end date for the report period in YYYY-MM-DD format.\"\n    },\n    \"store_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Optional list of store IDs to filter the report by specific stores.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current processing status of the report.\",\n      \"enum\": [\n        \"PENDING\",\n        \"PROCESSING\",\n        \"SUCCEEDED\",\n        \"FAILED\"\n      ]\n    },\n    \"download_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A temporary URL to download the completed report. Only present when status is SUCCEEDED.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"When the report request was created.\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the report generation completed. Only present when status is SUCCEEDED or FAILED.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/json-schema/doordash-report-schema.json
tags: []
title: DoorDash Report
---
