---
description: Request body for approving or recalling a report
layout: schema
name: ReportApproveRequest
properties_list:
- description: An optional comment accompanying the approval
  name: comment
  type: string
- description: Comment explaining why specific expenses are being rejected within an otherwise approved report
  name: expenseRejectedComment
  type: string
- description: Target status identifier
  name: statusId
  type: string
- description: The expected current workflow step code for optimistic concurrency control
  name: expectedStepCode
  type: string
- description: The expected current workflow step sequence number for optimistic concurrency control
  name: expectedStepSequence
  type: integer
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-report-approve-request-schema.json
slug: sap-concur-expense-report-approve-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportApproveRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for approving or recalling a report\",\n  \"properties\": {\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"An optional comment accompanying the approval\"\n    },\n    \"expenseRejectedComment\": {\n      \"type\": \"string\",\n      \"description\": \"Comment explaining why specific expenses are being rejected within an otherwise approved report\"\n    },\n    \"statusId\": {\n      \"type\": \"string\",\n      \"description\": \"Target status identifier\"\n    },\n    \"expectedStepCode\": {\n      \"type\": \"string\",\n      \"description\": \"The expected current workflow step code for optimistic concurrency control\"\n    },\n    \"expectedStepSequence\": {\n      \"type\": \"integer\",\n      \"description\": \"The expected current workflow step sequence number for optimistic\
  \ concurrency control\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-report-approve-request-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: ReportApproveRequest
---
