---
description: Represents a single disbursement line item from Affirm to the merchant, associated with a specific transaction event.
layout: schema
name: SettlementEvent
properties_list:
- description: A unique identifier for the settlement event.
  name: id
  type: string
- description: The identifier of the transaction this settlement event belongs to.
  name: transaction_id
  type: string
- description: The identifier of the specific transaction event that triggered this settlement.
  name: transaction_event_id
  type: string
- description: Net disbursement amount in the smallest currency unit.
  name: amount
  type: integer
- description: ISO 4217 currency code for this settlement.
  name: currency
  type: string
- description: Timestamp when this settlement event was created, in RFC 3339 format.
  name: created
  type: string
- description: The type of settlement event corresponding to the transaction action.
  name: type
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/transactions-settlement-event-schema.json
slug: transactions-settlement-event
source_filename: transactions-settlement-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/transactions-settlement-event-schema.json\",\n  \"title\": \"SettlementEvent\",\n  \"description\": \"Represents a single disbursement line item from Affirm to the merchant, associated with a specific transaction event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the settlement event.\",\n      \"example\": \"500123\"\n    },\n    \"transaction_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the transaction this settlement event belongs to.\",\n      \"example\": \"500123\"\n    },\n    \"transaction_event_id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the specific transaction event that triggered this settlement.\",\n      \"example\": \"500123\"\n\
  \    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Net disbursement amount in the smallest currency unit.\",\n      \"example\": 1\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for this settlement.\",\n      \"example\": \"USD\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when this settlement event was created, in RFC 3339 format.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of settlement event corresponding to the transaction action.\",\n      \"enum\": [\n        \"capture\",\n        \"refund\",\n        \"void\"\n      ],\n      \"example\": \"capture\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/transactions-settlement-event-schema.json
tags: []
title: SettlementEvent
---
