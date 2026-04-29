---
description: PaymentInstrument schema from Adyen API
layout: schema
name: PaymentInstrument
properties_list:
- description: The description of the resource.
  name: description
  type: string
- description: The unique identifier of the resource.
  name: id
  type: string
- description: The reference for the resource.
  name: reference
  type: string
- description: The type of wallet the network token is associated with.
  name: tokenType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-payment-instrument-schema.json
slug: transfer-webhooks-payment-instrument
source_filename: transfer-webhooks-payment-instrument-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-payment-instrument-schema.json\",\n  \"title\": \"PaymentInstrument\",\n  \"description\": \"PaymentInstrument schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"The description of the resource.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the resource.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"The reference for the resource.\",\n      \"type\": \"string\"\n    },\n    \"tokenType\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The type of wallet the network token is associated with.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-payment-instrument-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentInstrument
---
