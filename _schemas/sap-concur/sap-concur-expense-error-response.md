---
description: Standard error response
layout: schema
name: ErrorResponse
properties_list:
- description: Unique identifier for this error occurrence
  name: errorId
  type: string
- description: Human-readable error description
  name: errorMessage
  type: string
- description: The HTTP status code as a string
  name: httpStatus
  type: string
- description: The request path that triggered the error
  name: path
  type: string
- description: When the error occurred
  name: timestamp
  type: string
- description: Detailed field-level validation failures
  name: validationErrors
  type: array
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-error-response-schema.json
slug: sap-concur-expense-error-response
source_filename: sap-concur-expense-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response\",\n  \"properties\": {\n    \"errorId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this error occurrence\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error description\"\n    },\n    \"httpStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP status code as a string\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The request path that triggered the error\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"When the error occurred\"\n    },\n    \"validationErrors\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed field-level validation failures\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-error-response-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: ErrorResponse
---
