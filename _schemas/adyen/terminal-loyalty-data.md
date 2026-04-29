---
description: In the Payment, Loyalty or Balance Inquiry Request message, it allows the Sale Terminal to send the identification of the loyalty account or an awarded amount or an amount to redeem to the loyalty account. Data related to a Loyalty program or account.
layout: schema
name: LoyaltyData
properties_list:
- description: ''
  name: CardAcquisitionReference
  type: object
- description: ''
  name: LoyaltyAccountID
  type: object
- description: ''
  name: LoyaltyAmount
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-loyalty-data-schema.json
slug: terminal-loyalty-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-data-schema.json\",\n  \"title\": \"LoyaltyData\",\n  \"description\": \"In the Payment, Loyalty or Balance Inquiry Request message, it allows the Sale Terminal to send the identification of the loyalty account or an awarded amount or an amount to redeem to the loyalty account. Data related to a Loyalty program or account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CardAcquisitionReference\": {\n      \"$ref\": \"#/components/schemas/TransactionIDType\"\n    },\n    \"LoyaltyAccountID\": {\n      \"$ref\": \"#/components/schemas/LoyaltyAccountID\"\n    },\n    \"LoyaltyAmount\": {\n      \"$ref\": \"#/components/schemas/LoyaltyAmount\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoyaltyData
---
