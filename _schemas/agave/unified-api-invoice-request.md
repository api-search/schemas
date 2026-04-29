---
description: Request payload for creating an invoice.
layout: schema
name: InvoiceRequest
properties_list:
- description: Project to associate the invoice with.
  name: project_id
  type: string
- description: Vendor identifier.
  name: vendor_id
  type: string
- description: Vendor invoice number.
  name: invoice_number
  type: string
- description: Invoice amount in USD.
  name: amount
  type: number
- description: Invoice date.
  name: invoice_date
  type: string
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-invoice-request-schema.json
slug: unified-api-invoice-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-invoice-request-schema.json\",\n  \"title\": \"InvoiceRequest\",\n  \"description\": \"Request payload for creating an invoice.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"Project to associate the invoice with.\",\n      \"example\": \"proj-500123\"\n    },\n    \"vendor_id\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor identifier.\",\n      \"example\": \"ven-334455\"\n    },\n    \"invoice_number\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor invoice number.\",\n      \"example\": \"INV-2025-1042\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Invoice amount in USD.\",\n      \"example\": 85000.0\n    },\n    \"invoice_date\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date\",\n      \"description\": \"Invoice date.\",\n      \"example\": \"2025-03-01\"\n    }\n  },\n  \"required\": [\n    \"project_id\",\n    \"vendor_id\",\n    \"invoice_number\",\n    \"amount\",\n    \"invoice_date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-invoice-request-schema.json
tags:
- Accounting
- Construction
- Integration
title: InvoiceRequest
---
