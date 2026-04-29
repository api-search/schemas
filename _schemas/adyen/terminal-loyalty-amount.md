---
description: An awarded amount or an amount to redeem to the loyalty account might be sent in the Payment request message. Amount of a loyalty account.
layout: schema
name: LoyaltyAmount
properties_list:
- description: ''
  name: LoyaltyUnit
  type: object
- description: ''
  name: Currency
  type: string
- description: ''
  name: AmountValue
  type: number
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-loyalty-amount-schema.json
slug: terminal-loyalty-amount
source_filename: terminal-loyalty-amount-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-amount-schema.json\",\n  \"title\": \"LoyaltyAmount\",\n  \"description\": \"An awarded amount or an amount to redeem to the loyalty account might be sent in the Payment request message. Amount of a loyalty account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoyaltyUnit\": {\n      \"$ref\": \"#/components/schemas/LoyaltyUnit\"\n    },\n    \"Currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\"\n    },\n    \"AmountValue\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    }\n  },\n  \"required\": [\n    \"AmountValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-amount-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoyaltyAmount
---
