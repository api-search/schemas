---
description: Detailed information about a Bulk API 2.0 ingest job, including its current state and processing statistics.
layout: schema
name: IngestJobInfo
properties_list:
- description: The unique identifier of the ingest job.
  name: id
  type: string
- description: The DML operation being performed by this job.
  name: operation
  type: string
- description: The API name of the SObject type being processed.
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
- description: The number of records processed so far. Updated after processing completes.
  name: numberRecordsProcessed
  type: integer
- description: The number of records that failed during processing.
  name: numberRecordsFailed
  type: integer
- description: Total processing time in milliseconds.
  name: totalProcessingTime
  type: integer
- description: Error message if the job reached the Failed state. Describes the reason for failure.
  name: errorMessage
  type: string
- description: The content type of the data uploaded to this job.
  name: contentType
  type: string
- description: The line ending used in the uploaded data.
  name: lineEnding
  type: string
- description: The column delimiter used in the uploaded data.
  name: columnDelimiter
  type: string
- description: The external ID field name used for upsert operations. Only present for upsert jobs.
  name: externalIdFieldName
  type: string
- description: The job type (V2Ingest for Bulk API 2.0 ingest jobs).
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
schema_file: json-schema/salesforce-bulk-2-ingest-job-info-schema.json
slug: salesforce-bulk-2-ingest-job-info
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed information about a Bulk API 2.0 ingest job, including its current state and processing statistics.\\n\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the ingest job.\",\n      \"example\": \"abc123\"\n    },\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"The DML operation being performed by this job.\",\n      \"example\": \"insert\",\n      \"enum\": [\n        \"insert\",\n        \"update\",\n        \"upsert\",\n        \"delete\",\n        \"hardDelete\"\n      ]\n    },\n    \"object\": {\n      \"type\": \"string\",\n      \"description\": \"The API name of the SObject type being processed.\",\n      \"example\": \"example_value\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of a Bulk API 2.0 job, indicating where it is in its lifecycle.\\n\",\n      \"enum\"\
  : [\n        \"Open\",\n        \"UploadComplete\",\n        \"InProgress\",\n        \"JobComplete\",\n        \"Failed\",\n        \"Aborted\"\n      ]\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the job was created, in ISO 8601 format.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"systemModstamp\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the job was last modified, in ISO 8601 format.\\n\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"numberRecordsProcessed\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of records processed so far. Updated after processing completes.\\n\",\n      \"example\": 10\n    },\n    \"numberRecordsFailed\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of records that failed during processing.\",\n      \"example\": 10\n\
  \    },\n    \"totalProcessingTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Total processing time in milliseconds.\",\n      \"example\": 1700000000000\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if the job reached the Failed state. Describes the reason for failure.\\n\",\n      \"example\": \"example_value\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The content type of the data uploaded to this job.\",\n      \"example\": \"CSV\",\n      \"enum\": [\n        \"CSV\"\n      ]\n    },\n    \"lineEnding\": {\n      \"type\": \"string\",\n      \"description\": \"The line ending used in the uploaded data.\",\n      \"example\": \"LF\",\n      \"enum\": [\n        \"LF\",\n        \"CRLF\"\n      ]\n    },\n    \"columnDelimiter\": {\n      \"type\": \"string\",\n      \"description\": \"The column delimiter used in the uploaded data.\",\n      \"example\": \"COMMA\",\n\
  \      \"enum\": [\n        \"COMMA\",\n        \"TAB\",\n        \"PIPE\",\n        \"SEMICOLON\",\n        \"CARET\",\n        \"BACKQUOTE\"\n      ]\n    },\n    \"externalIdFieldName\": {\n      \"type\": \"string\",\n      \"description\": \"The external ID field name used for upsert operations. Only present for upsert jobs.\\n\",\n      \"example\": \"example_value\"\n    },\n    \"jobType\": {\n      \"type\": \"string\",\n      \"description\": \"The job type (V2Ingest for Bulk API 2.0 ingest jobs).\",\n      \"example\": \"example_value\"\n    },\n    \"createdById\": {\n      \"type\": \"string\",\n      \"description\": \"The Salesforce user ID of the user who created the job.\",\n      \"example\": \"500123\"\n    },\n    \"apiVersion\": {\n      \"type\": \"number\",\n      \"description\": \"The API version used to create the job.\",\n      \"example\": 42.5\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IngestJobInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-bulk-2-ingest-job-info-schema.json
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
title: IngestJobInfo
---
