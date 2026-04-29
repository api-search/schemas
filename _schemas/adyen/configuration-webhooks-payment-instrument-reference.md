---
description: PaymentInstrumentReference schema from Adyen API
layout: schema
name: PaymentInstrumentReference
properties_list:
- description: The unique identifier of the payment instrument.
  name: id
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-payment-instrument-reference-schema.json
slug: configuration-webhooks-payment-instrument-reference
source_filename: configuration-webhooks-payment-instrument-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-payment-instrument-reference-schema.json\",\n  \"title\": \"PaymentInstrumentReference\",\n  \"description\": \"PaymentInstrumentReference schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The unique identifier of the payment instrument.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-payment-instrument-reference-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentInstrumentReference
---
