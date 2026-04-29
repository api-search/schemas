---
description: LoyaltyAccountStatus schema from Adyen API
layout: schema
name: LoyaltyAccountStatus
properties_list:
- description: ''
  name: LoyaltyAccount
  type: object
- description: ''
  name: CurrentBalance
  type: number
- description: ''
  name: LoyaltyUnit
  type: object
- description: ''
  name: Currency
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-loyalty-account-status-schema.json
slug: terminal-loyalty-account-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-account-status-schema.json\",\n  \"title\": \"LoyaltyAccountStatus\",\n  \"description\": \"LoyaltyAccountStatus schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LoyaltyAccount\": {\n      \"$ref\": \"#/components/schemas/LoyaltyAccount\"\n    },\n    \"CurrentBalance\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"LoyaltyUnit\": {\n      \"$ref\": \"#/components/schemas/LoyaltyUnit\"\n    },\n    \"Currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\"\n    }\n  },\n  \"required\": [\n    \"LoyaltyAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-account-status-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoyaltyAccountStatus
---
