---
description: ListNetworkTokensResponse schema from Adyen API
layout: schema
name: ListNetworkTokensResponse
properties_list:
- description: List of network tokens.
  name: networkTokens
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-list-network-tokens-response-schema.json
slug: configuration-list-network-tokens-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-list-network-tokens-response-schema.json\",\n  \"title\": \"ListNetworkTokensResponse\",\n  \"description\": \"ListNetworkTokensResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"networkTokens\": {\n      \"description\": \"List of network tokens.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/NetworkToken\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-list-network-tokens-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ListNetworkTokensResponse
---
