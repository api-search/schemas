---
description: ResponseAdditionalDataNetworkTokens schema from Adyen API
layout: schema
name: ResponseAdditionalDataNetworkTokens
properties_list:
- description: Indicates whether a network token is available for the specified card.
  name: networkToken.available
  type: string
- description: The Bank Identification Number of a tokenized card, which is the first six digits of a card number.
  name: networkToken.bin
  type: string
- description: The last four digits of a network token.
  name: networkToken.tokenSummary
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-response-additional-data-network-tokens-schema.json
slug: payments-response-additional-data-network-tokens
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-response-additional-data-network-tokens-schema.json\",\n  \"title\": \"ResponseAdditionalDataNetworkTokens\",\n  \"description\": \"ResponseAdditionalDataNetworkTokens schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"networkToken.available\": {\n      \"description\": \"Indicates whether a network token is available for the specified card.\",\n      \"type\": \"string\"\n    },\n    \"networkToken.bin\": {\n      \"description\": \"The Bank Identification Number of a tokenized card, which is the first six digits of a card number.\",\n      \"type\": \"string\"\n    },\n    \"networkToken.tokenSummary\": {\n      \"description\": \"The last four digits of a network token.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-response-additional-data-network-tokens-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ResponseAdditionalDataNetworkTokens
---
