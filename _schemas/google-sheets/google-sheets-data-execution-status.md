---
description: The data execution status.
layout: schema
name: DataExecutionStatus
properties_list:
- description: The state of the data execution.
  name: state
  type: string
- description: The error code.
  name: errorCode
  type: string
- description: The error message, which may be empty.
  name: errorMessage
  type: string
- description: Gets the time the data last successfully refreshed.
  name: lastRefreshTime
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-data-execution-status-schema.json
slug: google-sheets-data-execution-status
source_filename: google-sheets-data-execution-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataExecutionStatus\",\n  \"type\": \"object\",\n  \"description\": \"The data execution status.\",\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the data execution.\"\n    },\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"The error code.\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"The error message, which may be empty.\"\n    },\n    \"lastRefreshTime\": {\n      \"type\": \"string\",\n      \"description\": \"Gets the time the data last successfully refreshed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-data-execution-status-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DataExecutionStatus
---
