---
description: Configuration parameters for creating a new Bulk API 2.0 query job.
layout: schema
name: QueryJobRequest
properties_list:
- description: The query operation to perform. Use query to retrieve active records only, or queryAll to include soft-deleted and archived records.
  name: operation
  type: string
- description: The SOQL query to execute. The query result will be available as CSV data after the job completes.
  name: query
  type: string
- description: The format of the results. Currently only CSV is supported.
  name: contentType
  type: string
- description: The delimiter character used between fields in the CSV output.
  name: columnDelimiter
  type: string
- description: The line ending character used in the CSV output.
  name: lineEnding
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-bulk-2-query-job-request-schema.json
slug: salesforce-bulk-2-query-job-request
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Configuration parameters for creating a new Bulk API 2.0 query job.\",\n  \"properties\": {\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"The query operation to perform. Use query to retrieve active records only, or queryAll to include soft-deleted and archived records.\\n\",\n      \"example\": \"query\",\n      \"enum\": [\n        \"query\",\n        \"queryAll\"\n      ]\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The SOQL query to execute. The query result will be available as CSV data after the job completes.\\n\",\n      \"example\": \"SELECT Id, Name, Email, Phone FROM Contact WHERE CreatedDate = LAST_YEAR\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The format of the results. Currently only CSV is supported.\",\n      \"example\": \"CSV\",\n      \"enum\": [\n        \"CSV\"\n      ]\n    },\n    \"columnDelimiter\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The delimiter character used between fields in the CSV output.\",\n      \"example\": \"COMMA\",\n      \"enum\": [\n        \"COMMA\",\n        \"TAB\",\n        \"PIPE\",\n        \"SEMICOLON\",\n        \"CARET\",\n        \"BACKQUOTE\"\n      ]\n    },\n    \"lineEnding\": {\n      \"type\": \"string\",\n      \"description\": \"The line ending character used in the CSV output.\",\n      \"example\": \"LF\",\n      \"enum\": [\n        \"LF\",\n        \"CRLF\"\n      ]\n    }\n  },\n  \"required\": [\n    \"operation\",\n    \"query\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QueryJobRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-bulk-2-query-job-request-schema.json
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
title: QueryJobRequest
---
