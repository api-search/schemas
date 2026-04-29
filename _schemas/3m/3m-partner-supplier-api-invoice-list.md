---
description: List of invoices
layout: schema
name: InvoiceList
properties_list:
- description: Array of invoice records
  name: invoices
  type: array
provider_name: 3M
provider_slug: 3m
schema_file: json-schema/3m-partner-supplier-api-invoice-list-schema.json
slug: 3m-partner-supplier-api-invoice-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-invoice-list-schema.json\",\n  \"title\": \"InvoiceList\",\n  \"description\": \"List of invoices\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invoices\": {\n      \"type\": \"array\",\n      \"description\": \"Array of invoice records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Invoice\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/3m/refs/heads/main/json-schema/3m-partner-supplier-api-invoice-list-schema.json
tags:
- Industrial
- Manufacturing
- Supply Chain
title: InvoiceList
---
