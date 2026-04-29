---
description: LoyaltyAccountReq schema from Adyen API
layout: schema
name: LoyaltyAccountReq
properties_list:
- description: ''
  name: CardAcquisitionReference
  type: object
- description: ''
  name: LoyaltyAccountID
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-loyalty-account-req-schema.json
slug: terminal-loyalty-account-req
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-account-req-schema.json\",\n  \"title\": \"LoyaltyAccountReq\",\n  \"description\": \"LoyaltyAccountReq schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CardAcquisitionReference\": {\n      \"$ref\": \"#/components/schemas/TransactionIDType\"\n    },\n    \"LoyaltyAccountID\": {\n      \"$ref\": \"#/components/schemas/LoyaltyAccountID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-account-req-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoyaltyAccountReq
---
