---
description: ActiveNetworkTokensRestriction schema from Adyen API
layout: schema
name: ActiveNetworkTokensRestriction
properties_list:
- description: Defines how the condition must be evaluated.
  name: operation
  type: string
- description: The number of tokens.
  name: value
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-active-network-tokens-restriction-schema.json
slug: configuration-active-network-tokens-restriction
source_filename: configuration-active-network-tokens-restriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-active-network-tokens-restriction-schema.json\",\n  \"title\": \"ActiveNetworkTokensRestriction\",\n  \"description\": \"ActiveNetworkTokensRestriction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"description\": \"Defines how the condition must be evaluated.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The number of tokens.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-active-network-tokens-restriction-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ActiveNetworkTokensRestriction
---
