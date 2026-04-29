---
description: ConvertedAmount schema from Adyen API
layout: schema
name: ConvertedAmount
properties_list:
- description: ''
  name: AmountValue
  type: number
- description: ''
  name: Currency
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-converted-amount-schema.json
slug: terminal-converted-amount
source_filename: terminal-converted-amount-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-converted-amount-schema.json\",\n  \"title\": \"ConvertedAmount\",\n  \"description\": \"ConvertedAmount schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AmountValue\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"Currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\"\n    }\n  },\n  \"required\": [\n    \"AmountValue\",\n    \"Currency\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-converted-amount-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ConvertedAmount
---
