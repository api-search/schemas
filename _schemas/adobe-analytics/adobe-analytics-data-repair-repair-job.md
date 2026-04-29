---
description: Status and details of a data repair job
layout: schema
name: RepairJob
properties_list:
- description: Unique job identifier
  name: jobId
  type: integer
- description: The report suite being repaired
  name: reportSuiteId
  type: string
- description: Start of the repair date range
  name: dateRangeStart
  type: string
- description: End of the repair date range
  name: dateRangeEnd
  type: string
- description: Current status of the repair job
  name: status
  type: string
- description: Job completion percentage (0-100)
  name: progress
  type: integer
- description: Timestamp when the job was created
  name: jobCreateTime
  type: string
- description: Timestamp when the job completed
  name: jobCompleteTime
  type: string
- description: Actual number of server calls processed
  name: serverCalls
  type: integer
- description: Number of data nodes processed
  name: nodesProcessed
  type: integer
provider_name: Adobe Analytics
provider_slug: adobe-analytics
schema_file: json-schema/adobe-analytics-data-repair-repair-job-schema.json
slug: adobe-analytics-data-repair-repair-job
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Status and details of a data repair job\",\n  \"properties\": {\n    \"jobId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique job identifier\",\n      \"example\": \"500123\"\n    },\n    \"reportSuiteId\": {\n      \"type\": \"string\",\n      \"description\": \"The report suite being repaired\",\n      \"example\": \"500123\"\n    },\n    \"dateRangeStart\": {\n      \"type\": \"string\",\n      \"description\": \"Start of the repair date range\",\n      \"format\": \"date\",\n      \"example\": \"2026-01-15\"\n    },\n    \"dateRangeEnd\": {\n      \"type\": \"string\",\n      \"description\": \"End of the repair date range\",\n      \"format\": \"date\",\n      \"example\": \"2026-01-15\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the repair job\",\n      \"example\": \"processing\",\n      \"enum\": [\n        \"processing\",\n        \"complete\"\
  ,\n        \"failed\"\n      ]\n    },\n    \"progress\": {\n      \"type\": \"integer\",\n      \"description\": \"Job completion percentage (0-100)\",\n      \"example\": 10\n    },\n    \"jobCreateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the job was created\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"jobCompleteTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the job completed\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"serverCalls\": {\n      \"type\": \"integer\",\n      \"description\": \"Actual number of server calls processed\",\n      \"example\": 10\n    },\n    \"nodesProcessed\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of data nodes processed\",\n      \"example\": 10\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RepairJob\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-analytics/refs/heads/main/json-schema/adobe-analytics-data-repair-repair-job-schema.json
tags:
- Adobe
- Analytics
- Business Intelligence
- Customer Intelligence
- Digital Marketing
- Marketing
- Web Analytics
title: RepairJob
---
