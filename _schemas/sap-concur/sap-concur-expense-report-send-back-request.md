---
description: Request body for sending a report back to the submitter
layout: schema
name: ReportSendBackRequest
properties_list:
- description: Explanation of why the report is being returned for corrections
  name: comment
  type: string
- description: The expected current workflow step code
  name: expectedStepCode
  type: string
- description: The expected current workflow step sequence number
  name: expectedStepSequence
  type: integer
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-report-send-back-request-schema.json
slug: sap-concur-expense-report-send-back-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportSendBackRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for sending a report back to the submitter\",\n  \"properties\": {\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Explanation of why the report is being returned for corrections\"\n    },\n    \"expectedStepCode\": {\n      \"type\": \"string\",\n      \"description\": \"The expected current workflow step code\"\n    },\n    \"expectedStepSequence\": {\n      \"type\": \"integer\",\n      \"description\": \"The expected current workflow step sequence number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-report-send-back-request-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: ReportSendBackRequest
---
