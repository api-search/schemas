---
description: CheckoutQrCodeAction schema from Adyen API
layout: schema
name: CheckoutQrCodeAction
properties_list:
- description: Expiry time of the QR code.
  name: expiresAt
  type: string
- description: Encoded payment data.
  name: paymentData
  type: string
- description: Specifies the payment method.
  name: paymentMethodType
  type: string
- description: The contents of the QR code as a UTF8 string.
  name: qrCodeData
  type: string
- description: '**qrCode**'
  name: type
  type: string
- description: Specifies the URL to redirect to.
  name: url
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-checkout-qr-code-action-schema.json
slug: checkout-checkout-qr-code-action
source_filename: checkout-checkout-qr-code-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-qr-code-action-schema.json\",\n  \"title\": \"CheckoutQrCodeAction\",\n  \"description\": \"CheckoutQrCodeAction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expiresAt\": {\n      \"description\": \"Expiry time of the QR code.\",\n      \"type\": \"string\"\n    },\n    \"paymentData\": {\n      \"description\": \"Encoded payment data.\",\n      \"type\": \"string\"\n    },\n    \"paymentMethodType\": {\n      \"description\": \"Specifies the payment method.\",\n      \"type\": \"string\"\n    },\n    \"qrCodeData\": {\n      \"description\": \"The contents of the QR code as a UTF8 string.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"**qrCode**\",\n      \"enum\": [\n        \"qrCode\"\n      ],\n      \"type\": \"string\"\n\
  \    },\n    \"url\": {\n      \"description\": \"Specifies the URL to redirect to.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-checkout-qr-code-action-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CheckoutQrCodeAction
---
