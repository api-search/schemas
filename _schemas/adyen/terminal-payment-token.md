---
description: Surrogate of the PAN (Primary Account Number) of the payment card to identify the payment mean of the customer. It allows, for a merchant, to identify the customer.
layout: schema
name: PaymentToken
properties_list:
- description: ''
  name: TokenRequestedType
  type: object
- description: ''
  name: TokenValue
  type: string
- description: Expiry date and time. Limits the validity of a payment token.
  name: ExpiryDateTime
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-payment-token-schema.json
slug: terminal-payment-token
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-token-schema.json\",\n  \"title\": \"PaymentToken\",\n  \"description\": \"Surrogate of the PAN (Primary Account Number) of the payment card to  identify the payment mean of the customer. It allows, for a merchant, to identify   the customer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TokenRequestedType\": {\n      \"$ref\": \"#/components/schemas/TokenRequestedType\"\n    },\n    \"TokenValue\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"ExpiryDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Expiry date and time. Limits the validity of a payment token.\"\n    }\n  },\n  \"required\": [\n    \"TokenRequestedType\",\n    \"TokenValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-token-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentToken
---
