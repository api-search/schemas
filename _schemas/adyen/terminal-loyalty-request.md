---
description: It conveys Information related to the Loyalty transaction to process. Content of the Loyalty Request message.
layout: schema
name: LoyaltyRequest
properties_list:
- description: ''
  name: SaleData
  type: object
- description: ''
  name: LoyaltyTransaction
  type: object
- description: ''
  name: LoyaltyData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-loyalty-request-schema.json
slug: terminal-loyalty-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-request-schema.json\",\n  \"title\": \"LoyaltyRequest\",\n  \"description\": \"It conveys Information related to the Loyalty transaction to process. Content of the Loyalty Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SaleData\": {\n      \"$ref\": \"#/components/schemas/SaleData\"\n    },\n    \"LoyaltyTransaction\": {\n      \"$ref\": \"#/components/schemas/LoyaltyTransaction\"\n    },\n    \"LoyaltyData\": {\n      \"$ref\": \"#/components/schemas/LoyaltyData\"\n    }\n  },\n  \"required\": [\n    \"SaleData\",\n    \"LoyaltyTransaction\",\n    \"LoyaltyData\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-loyalty-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: LoyaltyRequest
---
