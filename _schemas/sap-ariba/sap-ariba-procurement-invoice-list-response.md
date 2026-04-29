---
description: Paginated list of invoices
layout: schema
name: InvoiceListResponse
properties_list:
- description: Total number of matching invoices
  name: totalCount
  type: integer
- description: Number of records skipped
  name: skip
  type: integer
- description: Maximum records per page
  name: limit
  type: integer
- description: ''
  name: invoices
  type: array
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-invoice-list-response-schema.json
slug: sap-ariba-procurement-invoice-list-response
source_filename: sap-ariba-procurement-invoice-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InvoiceListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of invoices\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching invoices\"\n    },\n    \"skip\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records skipped\"\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum records per page\"\n    },\n    \"invoices\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-invoice-list-response-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: InvoiceListResponse
---
