---
description: ''
layout: schema
name: Invoice
properties_list:
- description: Unique document entry number
  name: DocEntry
  type: integer
- description: Document number
  name: DocNum
  type: integer
- description: Customer business partner code
  name: CardCode
  type: string
- description: Invoice date
  name: DocDate
  type: string
- description: Payment due date
  name: DocDueDate
  type: string
- description: Total invoice amount
  name: DocTotal
  type: number
- description: Invoice line items
  name: DocumentLines
  type: array
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-business-one-service-layer-invoice-schema.json
slug: sap-business-one-service-layer-invoice
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Invoice\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocEntry\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique document entry number\"\n    },\n    \"DocNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Document number\"\n    },\n    \"CardCode\": {\n      \"type\": \"string\",\n      \"description\": \"Customer business partner code\"\n    },\n    \"DocDate\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice date\"\n    },\n    \"DocDueDate\": {\n      \"type\": \"string\",\n      \"description\": \"Payment due date\"\n    },\n    \"DocTotal\": {\n      \"type\": \"number\",\n      \"description\": \"Total invoice amount\"\n    },\n    \"DocumentLines\": {\n      \"type\": \"array\",\n      \"description\": \"Invoice line items\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-business-one-service-layer-invoice-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: Invoice
---
