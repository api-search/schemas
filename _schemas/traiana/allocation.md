---
description: A trade allocation processed through the Traiana Harmony network, representing the distribution of a block trade to individual accounts.
layout: schema
name: Allocation
properties_list:
- description: Unique identifier for the allocation
  name: allocationId
  type: string
- description: Identifier of the parent block trade
  name: blockTradeId
  type: string
- description: Target account identifier for the allocation
  name: accountId
  type: string
- description: Instrument identifier or symbol
  name: instrument
  type: string
- description: Trade direction
  name: side
  type: string
- description: Allocated quantity
  name: quantity
  type: number
- description: Allocation price
  name: price
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Current status of the allocation
  name: status
  type: string
- description: Timestamp when the allocation was created
  name: createdAt
  type: string
provider_name: Traiana
provider_slug: traiana
schema_file: json-schema/allocation.json
slug: allocation
source_filename: allocation.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/allocation.json\",\n  \"title\": \"Allocation\",\n  \"description\": \"A trade allocation processed through the Traiana Harmony network, representing the distribution of a block trade to individual accounts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allocationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the allocation\"\n    },\n    \"blockTradeId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the parent block trade\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Target account identifier for the allocation\"\n    },\n    \"instrument\": {\n      \"type\": \"string\",\n      \"description\": \"Instrument identifier or symbol\"\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Trade direction\",\n      \"enum\": [\"Buy\", \"Sell\"]\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Allocated quantity\"\n    },\n    \"price\": {\n      \"type\": \"number\",\n      \"description\": \"Allocation price\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the allocation\",\n      \"enum\": [\"Pending\", \"Affirmed\", \"Confirmed\", \"Rejected\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the allocation was created\"\n    }\n  },\n  \"required\": [\"allocationId\", \"blockTradeId\", \"accountId\", \"instrument\", \"side\", \"quantity\", \"price\", \"currency\", \"status\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/allocation.json
tags:
- Fintech
- Foreign Exchange
- Post-Trade Processing
- Risk Management
title: Allocation
---
