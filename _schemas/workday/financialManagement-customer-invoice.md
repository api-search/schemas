---
description: ''
layout: schema
name: CustomerInvoice
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: invoiceNumber
  type: string
- description: ''
  name: invoiceDate
  type: string
- description: ''
  name: dueDate
  type: string
- description: ''
  name: totalAmount
  type: number
- description: ''
  name: status
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/financialManagement-customer-invoice-schema.json
slug: financialManagement-customer-invoice
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CustomerInvoice\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"invoiceNumber\": {\n      \"type\": \"string\"\n    },\n    \"invoiceDate\": {\n      \"type\": \"string\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\"\n    },\n    \"totalAmount\": {\n      \"type\": \"number\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/financialManagement-customer-invoice-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: CustomerInvoice
---
