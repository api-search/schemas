---
description: Represents a single event in the lifecycle of a transaction, such as an authorization, capture, refund, or void.
layout: schema
name: TransactionEvent
properties_list:
- description: A unique identifier for the transaction event.
  name: id
  type: string
- description: The type of transaction event.
  name: type
  type: string
- description: The amount associated with this event in the smallest currency unit.
  name: amount
  type: integer
- description: The ISO 4217 currency code for this event.
  name: currency
  type: string
- description: The fee charged by Affirm for this event in the smallest currency unit.
  name: fee
  type: integer
- description: The time when this event was created, in RFC 3339 format.
  name: created
  type: string
- description: An external reference identifier associated with this event.
  name: reference_id
  type: string
- description: Additional key-value metadata associated with this event for merchant tracking purposes.
  name: metadata
  type: object
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/transactions-transaction-event-schema.json
slug: transactions-transaction-event
source_filename: transactions-transaction-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/transactions-transaction-event-schema.json\",\n  \"title\": \"TransactionEvent\",\n  \"description\": \"Represents a single event in the lifecycle of a transaction, such as an authorization, capture, refund, or void.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the transaction event.\",\n      \"example\": \"500123\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of transaction event.\",\n      \"enum\": [\n        \"auth\",\n        \"capture\",\n        \"refund\",\n        \"void\",\n        \"update\"\n      ],\n      \"example\": \"auth\"\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount associated with this event in the smallest\
  \ currency unit.\",\n      \"example\": 1\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 4217 currency code for this event.\",\n      \"example\": \"USD\"\n    },\n    \"fee\": {\n      \"type\": \"integer\",\n      \"description\": \"The fee charged by Affirm for this event in the smallest currency unit.\",\n      \"example\": 1\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when this event was created, in RFC 3339 format.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"reference_id\": {\n      \"type\": \"string\",\n      \"description\": \"An external reference identifier associated with this event.\",\n      \"example\": \"500123\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Additional key-value metadata associated with this event for merchant tracking purposes.\",\n      \"additionalProperties\": {\n    \
  \    \"type\": \"string\"\n      },\n      \"example\": {}\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/transactions-transaction-event-schema.json
tags: []
title: TransactionEvent
---
