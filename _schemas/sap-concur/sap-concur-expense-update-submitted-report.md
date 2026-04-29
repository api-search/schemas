---
description: Limited-field JSON Merge Patch for updating a submitted report. Only accessible with Company JWT authentication.
layout: schema
name: UpdateSubmittedReport
properties_list:
- description: The name or title of the expense report
  name: name
  type: string
- description: The business justification
  name: businessPurpose
  type: string
- description: A comment to accompany the update
  name: comment
  type: string
- description: Whether physical receipts have been received
  name: isPaperReceiptsReceived
  type: boolean
- description: ''
  name: customData
  type: array
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-update-submitted-report-schema.json
slug: sap-concur-expense-update-submitted-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateSubmittedReport\",\n  \"type\": \"object\",\n  \"description\": \"Limited-field JSON Merge Patch for updating a submitted report. Only accessible with Company JWT authentication.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name or title of the expense report\"\n    },\n    \"businessPurpose\": {\n      \"type\": \"string\",\n      \"description\": \"The business justification\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"A comment to accompany the update\"\n    },\n    \"isPaperReceiptsReceived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether physical receipts have been received\"\n    },\n    \"customData\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-update-submitted-report-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: UpdateSubmittedReport
---
