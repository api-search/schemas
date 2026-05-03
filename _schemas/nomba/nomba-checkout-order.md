---
description: Schema representing a Nomba online checkout order for processing payments through multiple channels including Visa, Verve, Mastercard, USSD, bank transfers, and QR payments.
layout: schema
name: Nomba Checkout Order
properties_list:
- description: The payment amount for the checkout order.
  name: amount
  type: number
- description: The ISO 4217 currency code for the payment.
  name: currency
  type: string
- description: A unique merchant-provided reference for the order.
  name: orderReference
  type: string
- description: The email address of the customer making the payment.
  name: customerEmail
  type: string
- description: The URL to redirect the customer to after payment completion.
  name: callbackUrl
  type: string
- description: Whether to tokenize the customer card for future payments.
  name: tokenizeCard
  type: boolean
- description: The generated checkout URL to load in a browser for the customer to complete payment.
  name: checkoutLink
  type: string
- description: The current status of the checkout order.
  name: status
  type: string
- description: The date and time the order was created.
  name: createdAt
  type: string
provider_name: Nomba
provider_slug: nomba
schema_file: json-schema/nomba-checkout-order-schema.json
slug: nomba-checkout-order
source_filename: nomba-checkout-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.nomba.com/schemas/nomba/checkout-order.json\",\n  \"title\": \"Nomba Checkout Order\",\n  \"description\": \"Schema representing a Nomba online checkout order for processing payments through multiple channels including Visa, Verve, Mastercard, USSD, bank transfers, and QR payments.\",\n  \"type\": \"object\",\n  \"required\": [\"amount\", \"currency\", \"orderReference\"],\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"The payment amount for the checkout order.\",\n      \"minimum\": 1\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 4217 currency code for the payment.\",\n      \"enum\": [\"NGN\"]\n    },\n    \"orderReference\": {\n      \"type\": \"string\",\n      \"description\": \"A unique merchant-provided reference for the order.\",\n      \"minLength\": 1,\n      \"maxLength\"\
  : 100\n    },\n    \"customerEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the customer making the payment.\"\n    },\n    \"callbackUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to redirect the customer to after payment completion.\"\n    },\n    \"tokenizeCard\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to tokenize the customer card for future payments.\",\n      \"default\": false\n    },\n    \"checkoutLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The generated checkout URL to load in a browser for the customer to complete payment.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the checkout order.\",\n      \"enum\": [\"pending\", \"successful\", \"failed\", \"cancelled\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the order was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/json-schema/nomba-checkout-order-schema.json
tags:
- Payments
- Fintech
- Banking
- Transfers
- Virtual Accounts
- Checkout
- Cross-Border Payments
- Cards
title: Nomba Checkout Order
---
