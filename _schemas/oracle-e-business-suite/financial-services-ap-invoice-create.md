---
description: ''
layout: schema
name: ApInvoiceCreate
properties_list:
- description: ''
  name: invoiceNum
  type: string
- description: ''
  name: vendorId
  type: integer
- description: ''
  name: vendorSiteId
  type: integer
- description: ''
  name: invoiceAmount
  type: number
- description: ''
  name: invoiceCurrencyCode
  type: string
- description: ''
  name: invoiceDate
  type: string
- description: ''
  name: invoiceType
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: termsId
  type: integer
- description: ''
  name: source
  type: string
- description: ''
  name: lines
  type: array
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-ap-invoice-create-schema.json
slug: financial-services-ap-invoice-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApInvoiceCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invoiceNum\": {\n      \"type\": \"string\"\n    },\n    \"vendorId\": {\n      \"type\": \"integer\"\n    },\n    \"vendorSiteId\": {\n      \"type\": \"integer\"\n    },\n    \"invoiceAmount\": {\n      \"type\": \"number\"\n    },\n    \"invoiceCurrencyCode\": {\n      \"type\": \"string\"\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\"\n    },\n    \"invoiceType\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"termsId\": {\n      \"type\": \"integer\"\n    },\n    \"source\": {\n      \"type\": \"string\"\n    },\n    \"lines\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-ap-invoice-create-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: ApInvoiceCreate
---
