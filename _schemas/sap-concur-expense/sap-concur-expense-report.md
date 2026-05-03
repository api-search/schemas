---
description: Schema for an SAP Concur Expense Report, which aggregates individual expense entries submitted by an employee for approval and reimbursement.
layout: schema
name: SAP Concur Expense Report
properties_list:
- description: The unique identifier of the expense report
  name: ID
  type: string
- description: The name/title of the expense report
  name: Name
  type: string
- description: Total amount of all expenses in the report in the report currency
  name: Total
  type: number
- description: ISO 4217 three-letter currency code for the report total
  name: CurrencyCode
  type: string
- description: Current approval workflow status code
  name: ApprovalStatusCode
  type: string
- description: Human-readable approval status label
  name: ApprovalStatusName
  type: string
- description: Current payment processing status code
  name: PaymentStatusCode
  type: string
- description: Human-readable payment status label
  name: PaymentStatusName
  type: string
- description: ISO 8601 datetime when the report was submitted for approval
  name: SubmitDate
  type: string
- description: ISO 8601 datetime when the report was created
  name: CreateDate
  type: string
- description: ISO 8601 datetime when payment processing began
  name: ProcessingPaymentDate
  type: string
- description: Login ID (email) of the expense report owner
  name: OwnerLoginID
  type: string
- description: Full display name of the expense report owner
  name: OwnerName
  type: string
- description: Identifier of the expense policy applied to this report
  name: PolicyID
  type: string
- description: Human-readable sequential report number
  name: ReportNumber
  type: string
- description: True if the report contains entries with policy exceptions requiring justification
  name: HasException
  type: boolean
- description: Business purpose statement for the expenses in this report
  name: PurposeStatement
  type: string
- description: Full URI for the expense report resource
  name: URI
  type: string
provider_name: SAP Concur Expense
provider_slug: sap-concur-expense
schema_file: json-schema/sap-concur-expense-report-schema.json
slug: sap-concur-expense-report
source_filename: sap-concur-expense-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/sap-concur-expense/json-schema/sap-concur-expense-report-schema.json\",\n  \"title\": \"SAP Concur Expense Report\",\n  \"description\": \"Schema for an SAP Concur Expense Report, which aggregates individual expense entries submitted by an employee for approval and reimbursement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the expense report\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name/title of the expense report\",\n      \"maxLength\": 40\n    },\n    \"Total\": {\n      \"type\": \"number\",\n      \"description\": \"Total amount of all expenses in the report in the report currency\"\n    },\n    \"CurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 three-letter currency code for the report\
  \ total\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"ApprovalStatusCode\": {\n      \"type\": \"string\",\n      \"description\": \"Current approval workflow status code\",\n      \"enum\": [\n        \"A_AAFH\",\n        \"A_AAPH\",\n        \"A_ADMIN\",\n        \"A_APPR\",\n        \"A_EXTV\",\n        \"A_FILE\",\n        \"A_NOTF\",\n        \"A_PBDG\",\n        \"A_PECO\",\n        \"A_PEND\",\n        \"A_PVAL\",\n        \"A_RESU\",\n        \"A_RHLD\",\n        \"A_TEXP\"\n      ]\n    },\n    \"ApprovalStatusName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable approval status label\"\n    },\n    \"PaymentStatusCode\": {\n      \"type\": \"string\",\n      \"description\": \"Current payment processing status code\",\n      \"enum\": [\"P_HOLD\", \"P_NOTP\", \"P_PAID\", \"P_PAYC\", \"P_PROC\"]\n    },\n    \"PaymentStatusName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable payment status label\"\n    },\n    \"SubmitDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 datetime when the report was submitted for approval\"\n    },\n    \"CreateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 datetime when the report was created\"\n    },\n    \"ProcessingPaymentDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 datetime when payment processing began\"\n    },\n    \"OwnerLoginID\": {\n      \"type\": \"string\",\n      \"description\": \"Login ID (email) of the expense report owner\"\n    },\n    \"OwnerName\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name of the expense report owner\"\n    },\n    \"PolicyID\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the expense policy applied to this report\"\n    },\n    \"ReportNumber\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Human-readable sequential report number\"\n    },\n    \"HasException\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the report contains entries with policy exceptions requiring justification\"\n    },\n    \"PurposeStatement\": {\n      \"type\": \"string\",\n      \"description\": \"Business purpose statement for the expenses in this report\"\n    },\n    \"URI\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Full URI for the expense report resource\"\n    }\n  },\n  \"required\": [\"Name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur-expense/refs/heads/main/json-schema/sap-concur-expense-report-schema.json
tags:
- Expense Management
- Financial Management
- Receipts
- Reimbursement
- Reporting
- SAP
- Travel
title: SAP Concur Expense Report
---
