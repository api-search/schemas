---
description: A fill (execution) in the Bloomberg Execution Management System (EMSX) representing a completed or partial trade execution against a route. Fills contain execution price, quantity, broker, exchange, and settlement information.
layout: schema
name: Bloomberg EMSX Fill
properties_list:
- description: Unique fill identifier within the EMSX blotter
  name: fillId
  type: integer
- description: Parent order sequence number
  name: orderSequenceNumber
  type: integer
- description: Parent route identifier
  name: routeId
  type: integer
- description: Bloomberg security ticker symbol
  name: ticker
  type: string
- description: Side of the fill
  name: side
  type: string
- description: Executed quantity in this fill
  name: fillAmount
  type: number
- description: Execution price for this fill
  name: fillPrice
  type: number
- description: Bloomberg broker code of the executing broker
  name: broker
  type: string
- description: Full name of the executing broker
  name: brokerName
  type: string
- description: Exchange or venue where the execution occurred
  name: exchange
  type: string
- description: Trade currency in ISO 4217 three-letter code
  name: currency
  type: string
- description: Settlement date for the trade
  name: settlementDate
  type: string
- description: Trade date (date the execution occurred)
  name: tradeDate
  type: string
- description: ISO 8601 timestamp of the fill execution
  name: fillTime
  type: string
- description: Trading account identifier
  name: account
  type: string
- description: Whether this fill was manually entered (e.g., for voice-brokered trades)
  name: isManual
  type: boolean
- description: Counterparty identifier for the trade
  name: contraParty
  type: string
provider_name: Bloomberg EMSX
provider_slug: bloomberg-emsx
schema_file: json-schema/bloomberg-emsx-fill-schema.json
slug: bloomberg-emsx-fill
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.bloomberg.com/schemas/emsx/fill.json\",\n  \"title\": \"Bloomberg EMSX Fill\",\n  \"description\": \"A fill (execution) in the Bloomberg Execution Management System (EMSX) representing a completed or partial trade execution against a route. Fills contain execution price, quantity, broker, exchange, and settlement information.\",\n  \"type\": \"object\",\n  \"required\": [\"orderSequenceNumber\", \"routeId\", \"fillAmount\", \"fillPrice\"],\n  \"properties\": {\n    \"fillId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique fill identifier within the EMSX blotter\"\n    },\n    \"orderSequenceNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent order sequence number\"\n    },\n    \"routeId\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent route identifier\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Bloomberg security ticker symbol\"\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"enum\": [\"BUY\", \"SELL\", \"SHORT\", \"COVER\"],\n      \"description\": \"Side of the fill\"\n    },\n    \"fillAmount\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"exclusiveMinimum\": true,\n      \"description\": \"Executed quantity in this fill\"\n    },\n    \"fillPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Execution price for this fill\"\n    },\n    \"broker\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg broker code of the executing broker\"\n    },\n    \"brokerName\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the executing broker\"\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"Exchange or venue where the execution occurred\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"Trade\
  \ currency in ISO 4217 three-letter code\"\n    },\n    \"settlementDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Settlement date for the trade\"\n    },\n    \"tradeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Trade date (date the execution occurred)\"\n    },\n    \"fillTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the fill execution\"\n    },\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"Trading account identifier\"\n    },\n    \"isManual\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this fill was manually entered (e.g., for voice-brokered trades)\"\n    },\n    \"contraParty\": {\n      \"type\": \"string\",\n      \"description\": \"Counterparty identifier for the trade\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-emsx/refs/heads/main/json-schema/bloomberg-emsx-fill-schema.json
tags:
- Bloomberg
- Execution Management
- Financial Services
- Order Management
- Trading
title: Bloomberg EMSX Fill
---
