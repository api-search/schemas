---
description: A give-up message processed through the Traiana Harmony network, representing the transfer of a trade from an executing broker to a prime broker on behalf of a client.
layout: schema
name: Give-Up
properties_list:
- description: Unique identifier for the give-up message
  name: giveUpId
  type: string
- description: Identifier of the associated trade
  name: tradeId
  type: string
- description: Identifier of the executing broker
  name: executingBrokerId
  type: string
- description: Identifier of the prime broker
  name: primeBrokerId
  type: string
- description: Identifier of the client
  name: clientId
  type: string
- description: Instrument identifier or symbol
  name: instrument
  type: string
- description: Trade direction
  name: side
  type: string
- description: Trade quantity
  name: quantity
  type: number
- description: Execution price
  name: price
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Current status of the give-up
  name: status
  type: string
- description: Timestamp when the give-up was submitted
  name: createdAt
  type: string
provider_name: Traiana
provider_slug: traiana
schema_file: json-schema/give-up.json
slug: give-up
source_filename: give-up.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/give-up.json\",\n  \"title\": \"Give-Up\",\n  \"description\": \"A give-up message processed through the Traiana Harmony network, representing the transfer of a trade from an executing broker to a prime broker on behalf of a client.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"giveUpId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the give-up message\"\n    },\n    \"tradeId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the associated trade\"\n    },\n    \"executingBrokerId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the executing broker\"\n    },\n    \"primeBrokerId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the prime broker\"\n    },\n    \"clientId\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Identifier of the client\"\n    },\n    \"instrument\": {\n      \"type\": \"string\",\n      \"description\": \"Instrument identifier or symbol\"\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"description\": \"Trade direction\",\n      \"enum\": [\"Buy\", \"Sell\"]\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Trade quantity\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Execution price\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the give-up\",\n      \"enum\": [\"Pending\", \"Accepted\", \"Rejected\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the give-up was submitted\"\n    }\n  },\n  \"required\": [\"giveUpId\"\
  , \"tradeId\", \"executingBrokerId\", \"primeBrokerId\", \"clientId\", \"instrument\", \"side\", \"quantity\", \"price\", \"currency\", \"status\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/give-up.json
tags:
- Fintech
- Foreign Exchange
- Post-Trade Processing
- Risk Management
title: Give-Up
---
