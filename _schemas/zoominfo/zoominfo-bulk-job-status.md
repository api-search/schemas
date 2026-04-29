---
description: ''
layout: schema
name: BulkJobStatus
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: jobType
  type: string
- description: ''
  name: entityType
  type: string
- description: ''
  name: totalRecords
  type: integer
- description: ''
  name: totalPages
  type: integer
- description: ''
  name: successfulPagesCount
  type: integer
- description: ''
  name: successfulPages
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-bulk-job-status-schema.json
slug: zoominfo-bulk-job-status
source_filename: zoominfo-bulk-job-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"jobType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"entityType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"totalRecords\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"totalPages\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"successfulPagesCount\": {\n      \"type\": \"integer\",\n      \"example\": 250\n    },\n    \"successfulPages\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"jobType\",\n    \"entityType\",\n    \"totalRecords\",\n    \"totalPages\",\n    \"successfulPagesCount\",\n    \"successfulPages\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"BulkJobStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-bulk-job-status-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: BulkJobStatus
---
