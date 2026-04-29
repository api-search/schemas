---
description: An accounts payable invoice.
layout: schema
name: Invoice
properties_list:
- description: Invoice identifier.
  name: id
  type: string
- description: Associated project identifier.
  name: project_id
  type: string
- description: Vendor who issued the invoice.
  name: vendor_id
  type: string
- description: Vendor invoice number.
  name: invoice_number
  type: string
- description: Invoice total amount in USD.
  name: amount
  type: number
- description: Invoice processing status.
  name: status
  type: string
- description: Invoice date.
  name: invoice_date
  type: string
- description: Invoice due date.
  name: due_date
  type: string
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-invoice-schema.json
slug: unified-api-invoice
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-invoice-schema.json\",\n  \"title\": \"Invoice\",\n  \"description\": \"An accounts payable invoice.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice identifier.\",\n      \"example\": \"inv-667788\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated project identifier.\",\n      \"example\": \"proj-500123\"\n    },\n    \"vendor_id\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor who issued the invoice.\",\n      \"example\": \"ven-334455\"\n    },\n    \"invoice_number\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor invoice number.\",\n      \"example\": \"INV-2025-1042\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Invoice total amount in USD.\",\n      \"example\": 85000.0\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Invoice processing status.\",\n      \"enum\": [\n        \"draft\",\n        \"submitted\",\n        \"approved\",\n        \"paid\",\n        \"rejected\"\n      ],\n      \"example\": \"approved\"\n    },\n    \"invoice_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Invoice date.\",\n      \"example\": \"2025-03-01\"\n    },\n    \"due_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Invoice due date.\",\n      \"example\": \"2025-03-31\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-invoice-schema.json
tags:
- Accounting
- Construction
- Integration
title: Invoice
---
