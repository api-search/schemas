---
description: PaymentInstrumentRevealInfo schema from Adyen API
layout: schema
name: PaymentInstrumentRevealInfo
properties_list:
- description: The CVC2 value of the card.
  name: cvc
  type: string
- description: The expiration date of the card.
  name: expiration
  type: object
- description: The primary account number (PAN) of the card.
  name: pan
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-payment-instrument-reveal-info-schema.json
slug: configuration-payment-instrument-reveal-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-payment-instrument-reveal-info-schema.json\",\n  \"title\": \"PaymentInstrumentRevealInfo\",\n  \"description\": \"PaymentInstrumentRevealInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cvc\": {\n      \"description\": \"The CVC2 value of the card.\",\n      \"type\": \"string\"\n    },\n    \"expiration\": {\n      \"description\": \"The expiration date of the card.\",\n      \"$ref\": \"#/components/schemas/Expiry\"\n    },\n    \"pan\": {\n      \"description\": \"The primary account number (PAN) of the card.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"pan\",\n    \"expiration\",\n    \"cvc\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-payment-instrument-reveal-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentInstrumentRevealInfo
---
