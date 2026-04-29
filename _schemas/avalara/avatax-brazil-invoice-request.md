---
description: InvoiceRequest schema from Avalara API
layout: schema
name: InvoiceRequest
properties_list:
- description: Electronic document type
  name: invoiceType
  type: string
- description: ''
  name: companyId
  type: string
- description: ''
  name: transactionDate
  type: string
- description: ''
  name: buyer
  type: object
- description: ''
  name: lines
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/avatax-brazil-invoice-request-schema.json
slug: avatax-brazil-invoice-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-invoice-request-schema.json\",\n  \"title\": \"InvoiceRequest\",\n  \"description\": \"InvoiceRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invoiceType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NF-e\",\n        \"NFS-e\",\n        \"NFC-e\",\n        \"CT-e\"\n      ],\n      \"description\": \"Electronic document type\"\n    },\n    \"companyId\": {\n      \"type\": \"string\"\n    },\n    \"transactionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"buyer\": {\n      \"$ref\": \"#/components/schemas/BrazilParty\"\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InvoiceLine\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/avatax-brazil-invoice-request-schema.json
tags:
- Taxes
title: InvoiceRequest
---
