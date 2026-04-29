---
description: The full representation of an expense entry
layout: schema
name: ExpenseDetail
properties_list:
- description: Unique identifier of the expense
  name: expenseId
  type: string
- description: The date the transaction occurred
  name: transactionDate
  type: string
- description: Business justification, maximum 64 characters
  name: businessPurpose
  type: string
- description: The allocation status of this expense
  name: allocationState
  type: string
- description: Whether this is a non-reimbursable personal expense
  name: isPersonalExpense
  type: boolean
- description: Whether the expense has been rejected by an approver
  name: isExpenseRejected
  type: boolean
- description: Whether a physical receipt has been received
  name: isPaperReceiptReceived
  type: boolean
- description: Whether the expense has policy exceptions
  name: hasExceptions
  type: boolean
- description: Reference to a supplier invoice
  name: invoiceId
  type: string
- description: ''
  name: customData
  type: array
- description: When the expense was last modified (ISO 8601)
  name: lastModifiedDate
  type: string
- description: HATEOAS navigation links
  name: links
  type: array
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-expense-detail-schema.json
slug: sap-concur-expense-expense-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExpenseDetail\",\n  \"type\": \"object\",\n  \"description\": \"The full representation of an expense entry\",\n  \"properties\": {\n    \"expenseId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the expense\"\n    },\n    \"transactionDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date the transaction occurred\"\n    },\n    \"businessPurpose\": {\n      \"type\": \"string\",\n      \"description\": \"Business justification, maximum 64 characters\"\n    },\n    \"allocationState\": {\n      \"type\": \"string\",\n      \"description\": \"The allocation status of this expense\"\n    },\n    \"isPersonalExpense\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a non-reimbursable personal expense\"\n    },\n    \"isExpenseRejected\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the expense has\
  \ been rejected by an approver\"\n    },\n    \"isPaperReceiptReceived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a physical receipt has been received\"\n    },\n    \"hasExceptions\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the expense has policy exceptions\"\n    },\n    \"invoiceId\": {\n      \"type\": \"string\",\n      \"description\": \"Reference to a supplier invoice\"\n    },\n    \"customData\": {\n      \"type\": \"array\"\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"string\",\n      \"description\": \"When the expense was last modified (ISO 8601)\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"HATEOAS navigation links\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-expense-detail-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: ExpenseDetail
---
