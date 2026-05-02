---
description: A sales invoice in Microsoft Dynamics 365, representing a bill issued to a customer for goods or services.
layout: schema
name: Sales Invoice
properties_list:
- description: The unique identifier of the sales invoice.
  name: id
  type: string
- description: The sales invoice number.
  name: number
  type: string
- description: The invoice date.
  name: invoiceDate
  type: string
- description: The posting date.
  name: postingDate
  type: string
- description: The payment due date.
  name: dueDate
  type: string
- description: The unique identifier of the customer.
  name: customerId
  type: string
- description: The customer number.
  name: customerNumber
  type: string
- description: The name of the customer.
  name: customerName
  type: string
- description: The currency code for the invoice.
  name: currencyCode
  type: string
- description: The status of the sales invoice.
  name: status
  type: string
- description: The total amount excluding tax.
  name: totalAmountExcludingTax
  type: number
- description: The total amount including tax.
  name: totalAmountIncludingTax
  type: number
- description: The date and time the record was last modified.
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
schema_file: json-schema/sales-invoice.json
slug: sales-invoice
source_filename: sales-invoice.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/sales-invoice.json\",\n  \"title\": \"Sales Invoice\",\n  \"description\": \"A sales invoice in Microsoft Dynamics 365, representing a bill issued to a customer for goods or services.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the sales invoice.\",\n      \"readOnly\": true\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The sales invoice number.\"\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The invoice date.\"\n    },\n    \"postingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The posting date.\"\n    },\n    \"dueDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The payment due date.\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the customer.\"\n    },\n    \"customerNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The customer number.\"\n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the customer.\",\n      \"readOnly\": true\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"The currency code for the invoice.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the sales invoice.\",\n      \"readOnly\": true\n    },\n    \"totalAmountExcludingTax\": {\n      \"type\": \"number\",\n      \"description\": \"The total amount excluding tax.\",\n      \"readOnly\": true\n    },\n    \"totalAmountIncludingTax\": {\n \
  \     \"type\": \"number\",\n      \"description\": \"The total amount including tax.\",\n      \"readOnly\": true\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was last modified.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"customerNumber\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/sales-invoice.json
tags:
- CRM
- ERP
- Microsoft Dynamics
title: Sales Invoice
---
