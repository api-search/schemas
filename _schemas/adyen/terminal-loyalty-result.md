---
description: In the Message Response, the result of each loyalty brand transaction. Data related to the result of a processed loyalty transaction.
layout: schema
name: LoyaltyResult
properties_list:
- description: ''
  name: LoyaltyAccount
  type: object
- description: if known (provided by the card or an external host).
  name: CurrentBalance
  type: number
- description: ''
  name: LoyaltyAmount
  type: object
- description: ''
  name: LoyaltyAcquirerData
  type: object
- description: ''
  name: Rebates
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-loyalty-result-schema.json
slug: terminal-loyalty-result
source_filename: terminal-loyalty-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-result-schema.json\",\n  \"title\": \"LoyaltyResult\",\n  \"description\": \"In the Message Response, the result of each loyalty brand transaction. Data related to the result of a processed loyalty transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoyaltyAccount\": {\n      \"$ref\": \"#/components/schemas/LoyaltyAccount\"\n    },\n    \"CurrentBalance\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"if known (provided by the card or an external host).\"\n    },\n    \"LoyaltyAmount\": {\n      \"$ref\": \"#/components/schemas/LoyaltyAmount\"\n    },\n    \"LoyaltyAcquirerData\": {\n      \"$ref\": \"#/components/schemas/LoyaltyAcquirerData\"\n    },\n    \"Rebates\": {\n      \"$ref\": \"#/components/schemas/Rebates\"\
  \n    }\n  },\n  \"required\": [\n    \"LoyaltyAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoyaltyResult
---
