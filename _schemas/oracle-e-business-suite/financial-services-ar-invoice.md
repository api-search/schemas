---
description: ''
layout: schema
name: ArInvoice
properties_list:
- description: Customer transaction identifier
  name: customerTrxId
  type: integer
- description: Transaction number
  name: trxNumber
  type: string
- description: Transaction date
  name: trxDate
  type: string
- description: Customer identifier
  name: customerId
  type: integer
- description: Customer name
  name: customerName
  type: string
- description: Bill-to site use identifier
  name: billToSiteUseId
  type: integer
- description: Ship-to site use identifier
  name: shipToSiteUseId
  type: integer
- description: Invoice currency (ISO 4217)
  name: invoiceCurrencyCode
  type: string
- description: Transaction type
  name: trxType
  type: string
- description: Transaction amount
  name: amount
  type: number
- description: Remaining amount due
  name: amountDue
  type: number
- description: Transaction status
  name: status
  type: string
- description: Payment terms identifier
  name: termsId
  type: integer
- description: ''
  name: lines
  type: array
- description: ''
  name: orgId
  type: integer
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-ar-invoice-schema.json
slug: financial-services-ar-invoice
source_filename: financial-services-ar-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ArInvoice\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerTrxId\": {\n      \"type\": \"integer\",\n      \"description\": \"Customer transaction identifier\"\n    },\n    \"trxNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction number\"\n    },\n    \"trxDate\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction date\"\n    },\n    \"customerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Customer identifier\"\n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"Customer name\"\n    },\n    \"billToSiteUseId\": {\n      \"type\": \"integer\",\n      \"description\": \"Bill-to site use identifier\"\n    },\n    \"shipToSiteUseId\": {\n      \"type\": \"integer\",\n      \"description\": \"Ship-to site use identifier\"\n    },\n    \"invoiceCurrencyCode\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Invoice currency (ISO 4217)\"\n    },\n    \"trxType\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction type\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Transaction amount\"\n    },\n    \"amountDue\": {\n      \"type\": \"number\",\n      \"description\": \"Remaining amount due\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction status\"\n    },\n    \"termsId\": {\n      \"type\": \"integer\",\n      \"description\": \"Payment terms identifier\"\n    },\n    \"lines\": {\n      \"type\": \"array\"\n    },\n    \"orgId\": {\n      \"type\": \"integer\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-ar-invoice-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: ArInvoice
---
