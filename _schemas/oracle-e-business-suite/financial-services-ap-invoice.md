---
description: ''
layout: schema
name: ApInvoice
properties_list:
- description: Invoice unique identifier
  name: invoiceId
  type: integer
- description: Invoice number
  name: invoiceNum
  type: string
- description: Invoice date
  name: invoiceDate
  type: string
- description: Supplier/vendor identifier
  name: vendorId
  type: integer
- description: Supplier/vendor name
  name: vendorName
  type: string
- description: Vendor site identifier
  name: vendorSiteId
  type: integer
- description: Total invoice amount
  name: invoiceAmount
  type: number
- description: Invoice currency code (ISO 4217)
  name: invoiceCurrencyCode
  type: string
- description: Payment currency code
  name: paymentCurrencyCode
  type: string
- description: Currency exchange rate
  name: exchangeRate
  type: number
- description: Exchange rate type
  name: exchangeRateType
  type: string
- description: Exchange rate date
  name: exchangeDate
  type: string
- description: Payment terms identifier
  name: termsId
  type: integer
- description: Invoice description
  name: description
  type: string
- description: Invoice type lookup code
  name: invoiceType
  type: string
- description: Invoice source
  name: source
  type: string
- description: Payment status
  name: paymentStatusFlag
  type: string
- description: Approval status
  name: approvalStatus
  type: string
- description: Amount paid
  name: amountPaid
  type: number
- description: ''
  name: lines
  type: array
- description: Operating unit identifier
  name: orgId
  type: integer
- description: ''
  name: createdBy
  type: integer
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdatedBy
  type: integer
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-ap-invoice-schema.json
slug: financial-services-ap-invoice
source_filename: financial-services-ap-invoice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApInvoice\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invoiceId\": {\n      \"type\": \"integer\",\n      \"description\": \"Invoice unique identifier\"\n    },\n    \"invoiceNum\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice number\"\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice date\"\n    },\n    \"vendorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Supplier/vendor identifier\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"description\": \"Supplier/vendor name\"\n    },\n    \"vendorSiteId\": {\n      \"type\": \"integer\",\n      \"description\": \"Vendor site identifier\"\n    },\n    \"invoiceAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total invoice amount\"\n    },\n    \"invoiceCurrencyCode\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Invoice currency code (ISO 4217)\"\n    },\n    \"paymentCurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Payment currency code\"\n    },\n    \"exchangeRate\": {\n      \"type\": \"number\",\n      \"description\": \"Currency exchange rate\"\n    },\n    \"exchangeRateType\": {\n      \"type\": \"string\",\n      \"description\": \"Exchange rate type\"\n    },\n    \"exchangeDate\": {\n      \"type\": \"string\",\n      \"description\": \"Exchange rate date\"\n    },\n    \"termsId\": {\n      \"type\": \"integer\",\n      \"description\": \"Payment terms identifier\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice description\"\n    },\n    \"invoiceType\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice type lookup code\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice source\"\n    },\n    \"paymentStatusFlag\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Payment status\"\n    },\n    \"approvalStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Approval status\"\n    },\n    \"amountPaid\": {\n      \"type\": \"number\",\n      \"description\": \"Amount paid\"\n    },\n    \"lines\": {\n      \"type\": \"array\"\n    },\n    \"orgId\": {\n      \"type\": \"integer\",\n      \"description\": \"Operating unit identifier\"\n    },\n    \"createdBy\": {\n      \"type\": \"integer\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdatedBy\": {\n      \"type\": \"integer\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-ap-invoice-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: ApInvoice
---
