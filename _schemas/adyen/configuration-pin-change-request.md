---
description: PinChangeRequest schema from Adyen API
layout: schema
name: PinChangeRequest
properties_list:
- description: Symmetric session key encrypted under the public key.
  name: encryptedKey
  type: string
- description: The encrypted PIN block
  name: encryptedPinBlock
  type: string
- description: The unique identifier of the payment instrument.
  name: paymentInstrumentId
  type: string
- description: The token which is used to construct the pinblock.
  name: token
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-pin-change-request-schema.json
slug: configuration-pin-change-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-pin-change-request-schema.json\",\n  \"title\": \"PinChangeRequest\",\n  \"description\": \"PinChangeRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"encryptedKey\": {\n      \"description\": \"Symmetric session key encrypted under the public key.\",\n      \"type\": \"string\"\n    },\n    \"encryptedPinBlock\": {\n      \"description\": \"The encrypted PIN block\",\n      \"type\": \"string\"\n    },\n    \"paymentInstrumentId\": {\n      \"description\": \"The unique identifier of the payment instrument.\",\n      \"type\": \"string\"\n    },\n    \"token\": {\n      \"description\": \"The token which is used to construct the pinblock.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"paymentInstrumentId\",\n    \"encryptedKey\",\n    \"token\"\
  ,\n    \"encryptedPinBlock\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-pin-change-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PinChangeRequest
---
