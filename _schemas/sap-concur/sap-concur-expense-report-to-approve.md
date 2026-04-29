---
description: A summary of an expense report awaiting approval
layout: schema
name: ReportToApprove
properties_list:
- description: Unique identifier of the report
  name: reportId
  type: string
- description: The report name
  name: name
  type: string
- description: The report owner's user ID
  name: userId
  type: string
- description: Current approval status
  name: approvalStatus
  type: string
- description: When the report was submitted
  name: submitDate
  type: string
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-report-to-approve-schema.json
slug: sap-concur-expense-report-to-approve
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportToApprove\",\n  \"type\": \"object\",\n  \"description\": \"A summary of an expense report awaiting approval\",\n  \"properties\": {\n    \"reportId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the report\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The report name\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"The report owner's user ID\"\n    },\n    \"approvalStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current approval status\"\n    },\n    \"submitDate\": {\n      \"type\": \"string\",\n      \"description\": \"When the report was submitted\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-report-to-approve-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: ReportToApprove
---
