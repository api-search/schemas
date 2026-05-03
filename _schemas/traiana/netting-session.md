---
description: A netting session processed through Traiana NetLink, representing an aggregation and compression cycle for trades between counterparties to reduce settlement risk and optimize liquidity.
layout: schema
name: Netting Session
properties_list:
- description: Unique identifier for the netting session
  name: sessionId
  type: string
- description: Identifier of the first counterparty
  name: counterpartyIdA
  type: string
- description: Identifier of the second counterparty
  name: counterpartyIdB
  type: string
- description: Asset class being netted
  name: assetClass
  type: string
- description: Current status of the netting session
  name: status
  type: string
- description: Number of original trades included in the session
  name: originalTradeCount
  type: integer
- description: Number of netted trades produced
  name: nettedTradeCount
  type: integer
- description: Ratio of compression achieved
  name: compressionRatio
  type: number
- description: Scheduled execution time
  name: scheduledAt
  type: string
- description: Completion timestamp
  name: completedAt
  type: string
- description: Timestamp when the session was created
  name: createdAt
  type: string
provider_name: Traiana
provider_slug: traiana
schema_file: json-schema/netting-session.json
slug: netting-session
source_filename: netting-session.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/netting-session.json\",\n  \"title\": \"Netting Session\",\n  \"description\": \"A netting session processed through Traiana NetLink, representing an aggregation and compression cycle for trades between counterparties to reduce settlement risk and optimize liquidity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the netting session\"\n    },\n    \"counterpartyIdA\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the first counterparty\"\n    },\n    \"counterpartyIdB\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the second counterparty\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"description\": \"Asset class being netted\"\n    },\n\
  \    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the netting session\",\n      \"enum\": [\"Pending\", \"InProgress\", \"Completed\", \"Failed\"]\n    },\n    \"originalTradeCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of original trades included in the session\"\n    },\n    \"nettedTradeCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of netted trades produced\"\n    },\n    \"compressionRatio\": {\n      \"type\": \"number\",\n      \"description\": \"Ratio of compression achieved\"\n    },\n    \"scheduledAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled execution time\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Completion timestamp\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"\
  Timestamp when the session was created\"\n    }\n  },\n  \"required\": [\"sessionId\", \"counterpartyIdA\", \"counterpartyIdB\", \"assetClass\", \"status\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/traiana/refs/heads/main/json-schema/netting-session.json
tags:
- Fintech
- Foreign Exchange
- Post-Trade Processing
- Risk Management
title: Netting Session
---
