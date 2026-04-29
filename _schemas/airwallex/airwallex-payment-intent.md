---
description: An Airwallex payment intent representing a payment session for collecting customer payment.
layout: schema
name: PaymentIntent
properties_list:
- description: Unique payment intent identifier.
  name: id
  type: string
- description: Payment amount in the specified currency.
  name: amount
  type: number
- description: ISO 4217 currency code.
  name: currency
  type: string
- description: Merchant's own order identifier.
  name: merchant_order_id
  type: string
- description: Current payment intent status.
  name: status
  type: string
- description: Client secret for frontend SDK initialization.
  name: client_secret
  type: string
- description: Amount captured so far.
  name: captured_amount
  type: number
- description: Airwallex customer ID.
  name: customer_id
  type: string
- description: Payment method configuration options.
  name: payment_method_options
  type: object
- description: Statement descriptor shown on customer bank statement.
  name: descriptor
  type: string
- description: Arbitrary key-value metadata for the payment intent.
  name: metadata
  type: object
- description: Timestamp when the payment intent was created.
  name: created_at
  type: string
- description: Timestamp of last update.
  name: updated_at
  type: string
provider_name: Airwallex
provider_slug: airwallex
schema_file: json-schema/airwallex-payment-intent-schema.json
slug: airwallex-payment-intent
source_filename: airwallex-payment-intent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/json-schema/airwallex-payment-intent-schema.json\",\n  \"title\": \"PaymentIntent\",\n  \"description\": \"An Airwallex payment intent representing a payment session for collecting customer payment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique payment intent identifier.\",\n      \"example\": \"int_abc123def456\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Payment amount in the specified currency.\",\n      \"example\": 100.00\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code.\",\n      \"example\": \"USD\"\n    },\n    \"merchant_order_id\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant's own order identifier.\",\n      \"example\"\
  : \"order-20260419-001\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"CREATED\", \"REQUIRES_PAYMENT_METHOD\", \"REQUIRES_CUSTOMER_ACTION\", \"REQUIRES_CAPTURE\", \"SUCCEEDED\", \"CANCELLED\", \"EXPIRED\"],\n      \"description\": \"Current payment intent status.\",\n      \"example\": \"SUCCEEDED\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\",\n      \"description\": \"Client secret for frontend SDK initialization.\",\n      \"example\": \"cs_abc123\"\n    },\n    \"captured_amount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount captured so far.\",\n      \"example\": 100.00\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"Airwallex customer ID.\",\n      \"example\": \"cus_abc123\"\n    },\n    \"payment_method_options\": {\n      \"type\": \"object\",\n      \"description\": \"Payment method configuration options.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"Statement descriptor shown on customer bank statement.\",\n      \"example\": \"ACME Corp\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Arbitrary key-value metadata for the payment intent.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the payment intent was created.\",\n      \"example\": \"2026-04-19T10:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last update.\",\n      \"example\": \"2026-04-19T10:31:00Z\"\n    }\n  },\n  \"required\": [\"id\", \"amount\", \"currency\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airwallex/refs/heads/main/json-schema/airwallex-payment-intent-schema.json
tags:
- Cross-Border Payments
- FinTech
- Foreign Exchange
- Payments
- Global
- Embedded Finance
- Multi-Currency
title: PaymentIntent
---
