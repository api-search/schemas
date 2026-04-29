---
description: ''
layout: schema
name: Order
properties_list:
- description: Unique document entry number
  name: DocEntry
  type: integer
- description: Document number
  name: DocNum
  type: integer
- description: Business partner code
  name: CardCode
  type: string
- description: Document date
  name: DocDate
  type: string
- description: Document due date
  name: DocDueDate
  type: string
- description: Total document amount
  name: DocTotal
  type: number
- description: Document currency
  name: DocCurrency
  type: string
- description: Order line items
  name: DocumentLines
  type: array
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-business-one-service-layer-order-schema.json
slug: sap-business-one-service-layer-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocEntry\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique document entry number\"\n    },\n    \"DocNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Document number\"\n    },\n    \"CardCode\": {\n      \"type\": \"string\",\n      \"description\": \"Business partner code\"\n    },\n    \"DocDate\": {\n      \"type\": \"string\",\n      \"description\": \"Document date\"\n    },\n    \"DocDueDate\": {\n      \"type\": \"string\",\n      \"description\": \"Document due date\"\n    },\n    \"DocTotal\": {\n      \"type\": \"number\",\n      \"description\": \"Total document amount\"\n    },\n    \"DocCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Document currency\"\n    },\n    \"DocumentLines\": {\n      \"type\": \"array\",\n      \"description\": \"Order line items\"\n   \
  \ }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-business-one-service-layer-order-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: Order
---
