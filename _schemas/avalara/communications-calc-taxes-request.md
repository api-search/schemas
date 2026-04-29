---
description: CalcTaxesRequest schema from Avalara API
layout: schema
name: CalcTaxesRequest
properties_list:
- description: ''
  name: cmpn
  type: object
- description: Array of invoices to calculate taxes for
  name: inv
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-calc-taxes-request-schema.json
slug: communications-calc-taxes-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-calc-taxes-request-schema.json\",\n  \"title\": \"CalcTaxesRequest\",\n  \"description\": \"CalcTaxesRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"cmpn\",\n    \"inv\"\n  ],\n  \"properties\": {\n    \"cmpn\": {\n      \"$ref\": \"#/components/schemas/CompanyData\"\n    },\n    \"inv\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Invoice\"\n      },\n      \"description\": \"Array of invoices to calculate taxes for\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-calc-taxes-request-schema.json
tags:
- Taxes
title: CalcTaxesRequest
---
