---
description: ''
layout: schema
name: ArInvoiceCreate
properties_list:
- description: ''
  name: customerId
  type: integer
- description: ''
  name: trxDate
  type: string
- description: ''
  name: invoiceCurrencyCode
  type: string
- description: ''
  name: batchSourceName
  type: string
- description: ''
  name: billToSiteUseId
  type: integer
- description: ''
  name: shipToSiteUseId
  type: integer
- description: ''
  name: termsId
  type: integer
- description: ''
  name: lines
  type: array
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-ar-invoice-create-schema.json
slug: financial-services-ar-invoice-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ArInvoiceCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customerId\": {\n      \"type\": \"integer\"\n    },\n    \"trxDate\": {\n      \"type\": \"string\"\n    },\n    \"invoiceCurrencyCode\": {\n      \"type\": \"string\"\n    },\n    \"batchSourceName\": {\n      \"type\": \"string\"\n    },\n    \"billToSiteUseId\": {\n      \"type\": \"integer\"\n    },\n    \"shipToSiteUseId\": {\n      \"type\": \"integer\"\n    },\n    \"termsId\": {\n      \"type\": \"integer\"\n    },\n    \"lines\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-ar-invoice-create-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: ArInvoiceCreate
---
