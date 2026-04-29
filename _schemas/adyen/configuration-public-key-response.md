---
description: PublicKeyResponse schema from Adyen API
layout: schema
name: PublicKeyResponse
properties_list:
- description: The public key to be used for encrypting the symmetric session key.
  name: publicKey
  type: string
- description: The expiry date of the public key.
  name: publicKeyExpiryDate
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-public-key-response-schema.json
slug: configuration-public-key-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-public-key-response-schema.json\",\n  \"title\": \"PublicKeyResponse\",\n  \"description\": \"PublicKeyResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"publicKey\": {\n      \"description\": \"The public key to be used for encrypting the symmetric session key.\",\n      \"type\": \"string\"\n    },\n    \"publicKeyExpiryDate\": {\n      \"description\": \"The expiry date of the public key.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"publicKey\",\n    \"publicKeyExpiryDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-public-key-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PublicKeyResponse
---
