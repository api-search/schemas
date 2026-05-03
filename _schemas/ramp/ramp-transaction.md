---
description: Schema describing a Ramp card or bill transaction record returned by the Ramp Developer API.
layout: schema
name: Ramp Transaction
properties_list:
- description: Unique identifier of the transaction.
  name: id
  type: string
- description: Transaction amount in the original currency.
  name: amount
  type: number
- description: ISO 4217 currency code.
  name: currency_code
  type: string
- description: Merchant or vendor name as captured at point of sale.
  name: merchant_name
  type: string
- description: Merchant category code returned by the card network.
  name: merchant_category_code
  type: string
- description: Timestamp the transaction was initiated by the user.
  name: user_transaction_time
  type: string
- description: Transaction state.
  name: state
  type: string
- description: Ramp spend category identifier.
  name: sk_category_id
  type: integer
- description: Identifier of the card used.
  name: card_id
  type: string
- description: Identifier of the user that initiated the transaction.
  name: user_id
  type: string
- description: Memo attached to the transaction.
  name: memo
  type: string
provider_name: Ramp
provider_slug: ramp
schema_file: json-schema/ramp-transaction.json
slug: ramp-transaction
source_filename: ramp-transaction.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/json-schema/ramp-transaction.json\",\n  \"title\": \"Ramp Transaction\",\n  \"description\": \"Schema describing a Ramp card or bill transaction record returned by the Ramp Developer API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Unique identifier of the transaction.\" },\n    \"amount\": { \"type\": \"number\", \"description\": \"Transaction amount in the original currency.\" },\n    \"currency_code\": { \"type\": \"string\", \"description\": \"ISO 4217 currency code.\" },\n    \"merchant_name\": { \"type\": \"string\", \"description\": \"Merchant or vendor name as captured at point of sale.\" },\n    \"merchant_category_code\": { \"type\": \"string\", \"description\": \"Merchant category code returned by the card network.\" },\n    \"user_transaction_time\": {\
  \ \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Timestamp the transaction was initiated by the user.\" },\n    \"state\": { \"type\": \"string\", \"enum\": [\"CLEARED\", \"PENDING\", \"DECLINED\", \"ERROR\"], \"description\": \"Transaction state.\" },\n    \"sk_category_id\": { \"type\": \"integer\", \"description\": \"Ramp spend category identifier.\" },\n    \"card_id\": { \"type\": \"string\", \"description\": \"Identifier of the card used.\" },\n    \"user_id\": { \"type\": \"string\", \"description\": \"Identifier of the user that initiated the transaction.\" },\n    \"memo\": { \"type\": \"string\", \"description\": \"Memo attached to the transaction.\" }\n  },\n  \"required\": [\"id\", \"amount\", \"currency_code\", \"state\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/json-schema/ramp-transaction.json
tags:
- Finance
- Spend Management
- Corporate Cards
- Expense Management
- Accounts Payable
- Bill Pay
- Accounting
- Reimbursements
title: Ramp Transaction
---
