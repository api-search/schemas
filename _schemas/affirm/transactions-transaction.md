---
description: Represents an Affirm payment transaction, capturing the full lifecycle from authorization through capture, refund, and void operations.
layout: schema
name: Transaction
properties_list:
- description: A unique identifier representing the transaction.
  name: id
  type: string
- description: A unique identifier referencing the Checkout object that originated this transaction.
  name: checkout_id
  type: string
- description: Identifies the order within the merchant's order management system.
  name: order_id
  type: string
- description: Current state of the transaction.
  name: status
  type: string
- description: The original amount financed to the customer in this transaction, expressed in the smallest currency unit (e.g., cents for USD).
  name: amount
  type: integer
- description: The cumulative amount refunded back to the customer from this transaction, expressed in the smallest currency unit.
  name: amount_refunded
  type: integer
- description: Local transaction currency following ISO 4217 standards.
  name: currency
  type: string
- description: The time when the transaction was created, in RFC 3339 format.
  name: created
  type: string
- description: The time when the transaction authorization expires and can no longer be captured, in RFC 3339 format.
  name: authorization_expiration
  type: string
- description: A unique identifier of the provider financing the transaction.
  name: provider_id
  type: integer
- description: Indicates whether tax was paid by the provider (applicable to Affirm Connect only).
  name: remove_tax
  type: boolean
- description: Array of TransactionEvent objects documenting the transaction history.
  name: events
  type: array
- description: A JWT signing the JSON response. If PII is included, this token is also encrypted.
  name: token
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/transactions-transaction-schema.json
slug: transactions-transaction
source_filename: transactions-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/transactions-transaction-schema.json\",\n  \"title\": \"Transaction\",\n  \"description\": \"Represents an Affirm payment transaction, capturing the full lifecycle from authorization through capture, refund, and void operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier representing the transaction.\",\n      \"example\": \"500123\"\n    },\n    \"checkout_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier referencing the Checkout object that originated this transaction.\",\n      \"example\": \"500123\"\n    },\n    \"order_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the order within the merchant's order management system.\",\n      \"example\": \"500123\"\
  \n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the transaction.\",\n      \"enum\": [\n        \"authorized\",\n        \"captured\",\n        \"voided\",\n        \"refunded\",\n        \"partially_refunded\"\n      ],\n      \"example\": \"authorized\"\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"The original amount financed to the customer in this transaction, expressed in the smallest currency unit (e.g., cents for USD).\",\n      \"example\": 1\n    },\n    \"amount_refunded\": {\n      \"type\": \"integer\",\n      \"description\": \"The cumulative amount refunded back to the customer from this transaction, expressed in the smallest currency unit.\",\n      \"example\": 1\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Local transaction currency following ISO 4217 standards.\",\n      \"example\": \"USD\"\n    },\n    \"created\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"The time when the transaction was created, in RFC 3339 format.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"authorization_expiration\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the transaction authorization expires and can no longer be captured, in RFC 3339 format.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"provider_id\": {\n      \"type\": \"integer\",\n      \"description\": \"A unique identifier of the provider financing the transaction.\",\n      \"example\": 1\n    },\n    \"remove_tax\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether tax was paid by the provider (applicable to Affirm Connect only).\",\n      \"example\": true\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Array of TransactionEvent objects documenting the transaction history.\",\n      \"items\"\
  : {\n        \"$ref\": \"#/components/schemas/TransactionEvent\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"A JWT signing the JSON response. If PII is included, this token is also encrypted.\",\n      \"example\": \"abc123def456abc123def456abc123de\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/transactions-transaction-schema.json
tags: []
title: Transaction
---
