---
description: RevealPinRequest schema from Adyen API
layout: schema
name: RevealPinRequest
properties_list:
- description: Symmetric session key encrypted under the public key.
  name: encryptedKey
  type: string
- description: The unique identifier of the payment instrument.
  name: paymentInstrumentId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-reveal-pin-request-schema.json
slug: configuration-reveal-pin-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-reveal-pin-request-schema.json\",\n  \"title\": \"RevealPinRequest\",\n  \"description\": \"RevealPinRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encryptedKey\": {\n      \"description\": \"Symmetric session key encrypted under the public key.\",\n      \"type\": \"string\"\n    },\n    \"paymentInstrumentId\": {\n      \"description\": \"The unique identifier of the payment instrument.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"paymentInstrumentId\",\n    \"encryptedKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-reveal-pin-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RevealPinRequest
---
