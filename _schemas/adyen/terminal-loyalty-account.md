---
description: This data structure conveys the identification of the account and the associated loyalty brand. Data related to a loyalty account processed in the transaction.
layout: schema
name: LoyaltyAccount
properties_list:
- description: ''
  name: LoyaltyAccountID
  type: object
- description: If a card is analysed.
  name: LoyaltyBrand
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-loyalty-account-schema.json
slug: terminal-loyalty-account
source_filename: terminal-loyalty-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-account-schema.json\",\n  \"title\": \"LoyaltyAccount\",\n  \"description\": \"This data structure conveys the identification of the account and the associated loyalty brand. Data related to a loyalty account processed in the transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoyaltyAccountID\": {\n      \"$ref\": \"#/components/schemas/LoyaltyAccountID\"\n    },\n    \"LoyaltyBrand\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If a card is analysed.\"\n    }\n  },\n  \"required\": [\n    \"LoyaltyAccountID\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-account-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoyaltyAccount
---
