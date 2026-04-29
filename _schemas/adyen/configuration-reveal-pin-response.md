---
description: RevealPinResponse schema from Adyen API
layout: schema
name: RevealPinResponse
properties_list:
- description: The encrypted PIN block.
  name: encryptedPinBlock
  type: string
- description: The encrypted PIN block extraction token.
  name: token
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-reveal-pin-response-schema.json
slug: configuration-reveal-pin-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-reveal-pin-response-schema.json\",\n  \"title\": \"RevealPinResponse\",\n  \"description\": \"RevealPinResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encryptedPinBlock\": {\n      \"description\": \"The encrypted PIN block.\",\n      \"type\": \"string\"\n    },\n    \"token\": {\n      \"description\": \"The encrypted PIN block extraction token.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"encryptedPinBlock\",\n    \"token\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-reveal-pin-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RevealPinResponse
---
