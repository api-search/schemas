---
description: Detailed information about a Bulk API 2.0 query job, including its current state and processing statistics.
layout: schema
name: QueryJobInfo
properties_list:
- description: The unique identifier of the query job.
  name: id
  type: string
- description: The query operation being performed.
  name: operation
  type: string
- description: The primary SObject type in the SOQL query. Derived automatically from the query.
  name: object
  type: string
- description: The current state of a Bulk API 2.0 job, indicating where it is in its lifecycle.
  name: state
  type: string
- description: The date and time the job was created, in ISO 8601 format.
  name: createdDate
  type: string
- description: The date and time the job was last modified, in ISO 8601 format.
  name: systemModstamp
  type: string
- description: The number of records returned by the query.
  name: numberRecordsProcessed
  type: integer
- description: Total processing time in milliseconds.
  name: totalProcessingTime
  type: integer
- description: Error message if the job reached the Failed state. Describes the reason for failure.
  name: errorMessage
  type: string
- description: The content type of the query results.
  name: contentType
  type: string
- description: The column delimiter used in the results CSV.
  name: columnDelimiter
  type: string
- description: The line ending used in the results CSV.
  name: lineEnding
  type: string
- description: The job type (V2Query for Bulk API 2.0 query jobs).
  name: jobType
  type: string
- description: The Salesforce user ID of the user who created the job.
  name: createdById
  type: string
- description: The API version used to create the job.
  name: apiVersion
  type: number
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-bulk-2-query-job-info-schema.json
slug: salesforce-bulk-2-query-job-info
source_filename: salesforce-bulk-2-query-job-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed information about a Bulk API 2.0 query job, including its current state and processing statistics.\\n\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the query job.\",\n      \"example\": \"abc123\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"The query operation being performed.\",\n      \"example\": \"query\",\n      \"enum\": [\n        \"query\",\n        \"queryAll\"\n      ]\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The primary SObject type in the SOQL query. Derived automatically from the query.\\n\",\n      \"example\": \"example_value\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of a Bulk API 2.0 job, indicating where it is in its lifecycle.\\n\",\n      \"enum\": [\n        \"Open\",\n        \"UploadComplete\"\
  ,\n        \"InProgress\",\n        \"JobComplete\",\n        \"Failed\",\n        \"Aborted\"\n      ]\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the job was created, in ISO 8601 format.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"systemModstamp\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the job was last modified, in ISO 8601 format.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"numberRecordsProcessed\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of records returned by the query.\",\n      \"example\": 10\n    },\n    \"totalProcessingTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Total processing time in milliseconds.\",\n      \"example\": 1700000000000\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Error message if the job reached the Failed state. Describes the reason for failure.\\n\",\n      \"example\": \"example_value\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The content type of the query results.\",\n      \"example\": \"CSV\",\n      \"enum\": [\n        \"CSV\"\n      ]\n    },\n    \"columnDelimiter\": {\n      \"type\": \"string\",\n      \"description\": \"The column delimiter used in the results CSV.\",\n      \"example\": \"COMMA\",\n      \"enum\": [\n        \"COMMA\",\n        \"TAB\",\n        \"PIPE\",\n        \"SEMICOLON\",\n        \"CARET\",\n        \"BACKQUOTE\"\n      ]\n    },\n    \"lineEnding\": {\n      \"type\": \"string\",\n      \"description\": \"The line ending used in the results CSV.\",\n      \"example\": \"LF\",\n      \"enum\": [\n        \"LF\",\n        \"CRLF\"\n      ]\n    },\n    \"jobType\": {\n      \"type\": \"string\",\n      \"description\": \"The job type (V2Query for Bulk API 2.0 query\
  \ jobs).\",\n      \"example\": \"example_value\"\n    },\n    \"createdById\": {\n      \"type\": \"string\",\n      \"description\": \"The Salesforce user ID of the user who created the job.\",\n      \"example\": \"500123\"\n    },\n    \"apiVersion\": {\n      \"type\": \"number\",\n      \"description\": \"The API version used to create the job.\",\n      \"example\": 42.5\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryJobInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-bulk-2-query-job-info-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: QueryJobInfo
---
