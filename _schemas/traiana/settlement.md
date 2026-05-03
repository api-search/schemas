---
description: A settlement instruction generated from Traiana NetLink netting sessions, representing PvP settlement orchestration for FX and other asset classes.
layout: schema
name: Settlement
properties_list:
- description: Unique identifier for the settlement instruction
  name: settlementId
  type: string
- description: Identifier of the originating netting session
  name: nettingSessionId
  type: string
- description: Identifier of the counterparty
  name: counterpartyId
  type: string
- description: Currency pair being settled
  name: currencyPair
  type: string
- description: Amount to be paid
  name: payAmount
  type: number
- description: ISO 4217 currency code for the pay leg
  name: payCurrency
  type: string
- description: Amount to be received
  name: receiveAmount
  type: number
- description: ISO 4217 currency code for the receive leg
  name: receiveCurrency
  type: string
- description: Settlement value date
  name: settlementDate
  type: string
- description: Current settlement status
  name: status
  type: string
- description: Timestamp when settlement was completed
  name: settledAt
  type: string
- description: Timestamp when the instruction was created
  name: createdAt
  type: string
provider_name: Traiana
provider_slug: traiana
schema_file: json-schema/settlement.json
slug: settlement
source_filename: settlement.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/settlement.json\",\n  \"title\": \"Settlement\",\n  \"description\": \"A settlement instruction generated from Traiana NetLink netting sessions, representing PvP settlement orchestration for FX and other asset classes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"settlementId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the settlement instruction\"\n    },\n    \"nettingSessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the originating netting session\"\n    },\n    \"counterpartyId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the counterparty\"\n    },\n    \"currencyPair\": {\n      \"type\": \"string\",\n      \"description\": \"Currency pair being settled\"\n    },\n    \"payAmount\": {\n      \"type\"\
  : \"number\",\n      \"description\": \"Amount to be paid\"\n    },\n    \"payCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the pay leg\"\n    },\n    \"receiveAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Amount to be received\"\n    },\n    \"receiveCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code for the receive leg\"\n    },\n    \"settlementDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Settlement value date\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current settlement status\",\n      \"enum\": [\"Pending\", \"Instructed\", \"Settled\", \"Failed\"]\n    },\n    \"settledAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when settlement was completed\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"Timestamp when the instruction was created\"\n    }\n  },\n  \"required\": [\"settlementId\", \"counterpartyId\", \"currencyPair\", \"payAmount\", \"payCurrency\", \"receiveAmount\", \"receiveCurrency\", \"settlementDate\", \"status\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/settlement.json
tags:
- Fintech
- Foreign Exchange
- Post-Trade Processing
- Risk Management
title: Settlement
---
