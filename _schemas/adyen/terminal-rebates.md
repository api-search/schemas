---
description: Rebates schema from Adyen API
layout: schema
name: Rebates
properties_list:
- description: ''
  name: TotalRebate
  type: number
- description: ''
  name: RebateLabel
  type: string
- description: ''
  name: SaleItemRebate
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-rebates-schema.json
slug: terminal-rebates
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-rebates-schema.json\",\n  \"title\": \"Rebates\",\n  \"description\": \"Rebates schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TotalRebate\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"RebateLabel\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"SaleItemRebate\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SaleItemRebate\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-rebates-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Rebates
---
