---
description: CalcTaxesResponse schema from Avalara API
layout: schema
name: CalcTaxesResponse
properties_list:
- description: ''
  name: inv
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-calc-taxes-response-schema.json
slug: communications-calc-taxes-response
source_filename: communications-calc-taxes-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-calc-taxes-response-schema.json\",\n  \"title\": \"CalcTaxesResponse\",\n  \"description\": \"CalcTaxesResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inv\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/InvoiceResult\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-calc-taxes-response-schema.json
tags:
- Taxes
title: CalcTaxesResponse
---
