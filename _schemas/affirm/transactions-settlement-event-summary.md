---
description: An aggregated summary of settlement activity for a single disbursement batch from Affirm to the merchant.
layout: schema
name: SettlementEventSummary
properties_list:
- description: A unique identifier for this settlement event summary.
  name: id
  type: string
- description: Total amount disbursed in this batch in the smallest currency unit.
  name: total_amount
  type: integer
- description: ISO 4217 currency code for this disbursement.
  name: currency
  type: string
- description: Number of individual settlement events included in this batch.
  name: event_count
  type: integer
- description: Timestamp when the disbursement was initiated, in RFC 3339 format.
  name: disbursed_at
  type: string
provider_name: affirm
provider_slug: affirm
schema_file: json-schema/transactions-settlement-event-summary-schema.json
slug: transactions-settlement-event-summary
source_filename: transactions-settlement-event-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/transactions-settlement-event-summary-schema.json\",\n  \"title\": \"SettlementEventSummary\",\n  \"description\": \"An aggregated summary of settlement activity for a single disbursement batch from Affirm to the merchant.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this settlement event summary.\",\n      \"example\": \"500123\"\n    },\n    \"total_amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total amount disbursed in this batch in the smallest currency unit.\",\n      \"example\": 1\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for this disbursement.\",\n      \"example\": \"USD\"\n    },\n    \"event_count\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Number of individual settlement events included in this batch.\",\n      \"example\": 1\n    },\n    \"disbursed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the disbursement was initiated, in RFC 3339 format.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/affirm/refs/heads/main/json-schema/transactions-settlement-event-summary-schema.json
tags: []
title: SettlementEventSummary
---
