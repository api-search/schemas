---
description: ''
layout: schema
name: BulkJobResultsRequest
properties_list:
- description: ''
  name: jobId
  type: string
- description: ''
  name: page
  type: integer
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-bulk-job-results-request-schema.json
slug: zoominfo-bulk-job-results-request
source_filename: zoominfo-bulk-job-results-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    }\n  },\n  \"required\": [\n    \"jobId\",\n    \"page\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BulkJobResultsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-bulk-job-results-request-schema.json
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
title: BulkJobResultsRequest
---
