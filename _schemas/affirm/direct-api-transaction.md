---
description: Represents an Affirm payment transaction at any point in its lifecycle.
layout: schema
name: Transaction
properties_list:
- description: Unique identifier for this transaction.
  name: id
  type: string
- description: Identifier of the checkout session that originated this transaction.
  name: checkout_id
  type: string
- description: Merchant's internal order identifier.
  name: order_id
  type: string
- description: Current lifecycle status of the transaction.
  name: status
  type: string
- description: Original authorized amount in cents.
  name: amount
  type: integer
- description: Cumulative amount refunded in cents.
  name: amount_refunded
  type: integer
- description: ISO 4217 currency code.
  name: currency
  type: string
- description: Creation timestamp in RFC 3339 format.
  name: created
  type: string
- description: Timestamp after which the authorization can no longer be captured.
  name: authorization_expiration
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/direct-api-transaction-schema.json
slug: direct-api-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/direct-api-transaction-schema.json\",\n  \"title\": \"Transaction\",\n  \"description\": \"Represents an Affirm payment transaction at any point in its lifecycle.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this transaction.\",\n      \"example\": \"500123\"\n    },\n    \"checkout_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the checkout session that originated this transaction.\",\n      \"example\": \"500123\"\n    },\n    \"order_id\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant's internal order identifier.\",\n      \"example\": \"500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the transaction.\"\
  ,\n      \"enum\": [\n        \"authorized\",\n        \"captured\",\n        \"voided\",\n        \"refunded\",\n        \"partially_refunded\"\n      ],\n      \"example\": \"authorized\"\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Original authorized amount in cents.\",\n      \"example\": 1\n    },\n    \"amount_refunded\": {\n      \"type\": \"integer\",\n      \"description\": \"Cumulative amount refunded in cents.\",\n      \"example\": 1\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code.\",\n      \"example\": \"USD\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp in RFC 3339 format.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"authorization_expiration\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp after which the authorization\
  \ can no longer be captured.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/direct-api-transaction-schema.json
tags: []
title: Transaction
---
