---
description: A trading order within Bloomberg AIM/EMSX, representing an instruction to buy or sell a financial instrument with specified parameters.
layout: schema
name: Order
properties_list:
- description: Unique EMSX order sequence number assigned by the system
  name: sequenceNumber
  type: integer
- description: Bloomberg security identifier for the order
  name: ticker
  type: string
- description: Order side indicating direction of the trade
  name: side
  type: string
- description: Total order quantity (shares or contracts)
  name: amount
  type: integer
- description: Type of order determining execution behavior
  name: orderType
  type: string
- description: Limit price for LMT and STP LMT orders
  name: limitPrice
  type: number
- description: Stop trigger price for STP and STP LMT orders
  name: stopPrice
  type: number
- description: Duration the order remains active
  name: timeInForce
  type: string
- description: Expiry date for Good-Till-Date orders
  name: gtdDate
  type: string
- description: Current order status
  name: status
  type: string
- description: Cumulative quantity filled across all routes
  name: filledAmount
  type: integer
- description: Quantity currently working (routed but not yet filled)
  name: workingAmount
  type: integer
- description: Volume-weighted average fill price
  name: averagePrice
  type: number
- description: Trading account identifier
  name: account
  type: string
- description: Portfolio name associated with the order
  name: portfolio
  type: string
- description: Trader responsible for the order
  name: trader
  type: string
- description: UUID of the assigned trader
  name: traderUuid
  type: string
- description: Name of the basket this order belongs to
  name: basketName
  type: string
- description: Handling instruction for the order
  name: handInstruction
  type: string
- description: Investor identifier for allocation purposes
  name: investorId
  type: string
- description: Free-text notes attached to the order
  name: notes
  type: string
- description: Custom note field 1
  name: customNote1
  type: string
- description: Custom note field 2
  name: customNote2
  type: string
- description: Custom note field 3
  name: customNote3
  type: string
- description: Custom note field 4
  name: customNote4
  type: string
- description: Custom note field 5
  name: customNote5
  type: string
- description: Whether this is a contract for difference order
  name: cfdFlag
  type: boolean
- description: Locate broker for short sell orders
  name: locateBroker
  type: string
- description: Locate ID for short sell orders
  name: locateId
  type: string
- description: Date the order was created
  name: createdDate
  type: string
- description: Timestamp of last order update
  name: lastUpdated
  type: string
- description: Routes associated with this order
  name: routes
  type: array
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/order.json
slug: order
source_filename: order.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://bloomberg.com/schemas/order.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Order\",\n  \"description\": \"A trading order within Bloomberg AIM/EMSX, representing an instruction to buy or sell a financial instrument with specified parameters.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"sequenceNumber\",\n    \"ticker\",\n    \"side\",\n    \"amount\",\n    \"orderType\",\n    \"timeInForce\"\n  ],\n  \"properties\": {\n    \"sequenceNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique EMSX order sequence number assigned by the system\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg security identifier for the order\",\n      \"examples\": [\n        \"IBM US Equity\",\n        \"AAPL US Equity\"\n      ]\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"description\": \"Order side indicating direction of the trade\",\n \
  \     \"enum\": [\n        \"BUY\",\n        \"SELL\",\n        \"SHRT\"\n      ]\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total order quantity (shares or contracts)\",\n      \"minimum\": 1\n    },\n    \"orderType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of order determining execution behavior\",\n      \"enum\": [\n        \"MKT\",\n        \"LMT\",\n        \"STP\",\n        \"STP LMT\"\n      ]\n    },\n    \"limitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Limit price for LMT and STP LMT orders\"\n    },\n    \"stopPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Stop trigger price for STP and STP LMT orders\"\n    },\n    \"timeInForce\": {\n      \"type\": \"string\",\n      \"description\": \"Duration the order remains active\",\n      \"enum\": [\n        \"DAY\",\n        \"GTC\",\n        \"OPG\",\n        \"IOC\",\n        \"FOK\",\n        \"GTD\",\n        \"MOC\",\n\
  \        \"LOC\"\n      ]\n    },\n    \"gtdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Expiry date for Good-Till-Date orders\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current order status\",\n      \"enum\": [\n        \"ASSIGN\",\n        \"CANCEL\",\n        \"CONNECTED\",\n        \"CXL_PND\",\n        \"DONE\",\n        \"EXPIRED\",\n        \"FILL\",\n        \"MOD_PND\",\n        \"NEW\",\n        \"PART_FILL\",\n        \"RJCT\",\n        \"SENT\",\n        \"WORKING\"\n      ]\n    },\n    \"filledAmount\": {\n      \"type\": \"integer\",\n      \"description\": \"Cumulative quantity filled across all routes\",\n      \"minimum\": 0,\n      \"default\": 0\n    },\n    \"workingAmount\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity currently working (routed but not yet filled)\",\n      \"minimum\": 0,\n      \"default\": 0\n    },\n    \"averagePrice\": {\n      \"\
  type\": \"number\",\n      \"description\": \"Volume-weighted average fill price\"\n    },\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"Trading account identifier\"\n    },\n    \"portfolio\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio name associated with the order\"\n    },\n    \"trader\": {\n      \"type\": \"string\",\n      \"description\": \"Trader responsible for the order\"\n    },\n    \"traderUuid\": {\n      \"type\": \"string\",\n      \"description\": \"UUID of the assigned trader\"\n    },\n    \"basketName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the basket this order belongs to\"\n    },\n    \"handInstruction\": {\n      \"type\": \"string\",\n      \"description\": \"Handling instruction for the order\",\n      \"enum\": [\n        \"ANY\",\n        \"DIR\",\n        \"FCM\"\n      ]\n    },\n    \"investorId\": {\n      \"type\": \"string\",\n      \"description\": \"Investor identifier\
  \ for allocation purposes\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Free-text notes attached to the order\"\n    },\n    \"customNote1\": {\n      \"type\": \"string\",\n      \"description\": \"Custom note field 1\"\n    },\n    \"customNote2\": {\n      \"type\": \"string\",\n      \"description\": \"Custom note field 2\"\n    },\n    \"customNote3\": {\n      \"type\": \"string\",\n      \"description\": \"Custom note field 3\"\n    },\n    \"customNote4\": {\n      \"type\": \"string\",\n      \"description\": \"Custom note field 4\"\n    },\n    \"customNote5\": {\n      \"type\": \"string\",\n      \"description\": \"Custom note field 5\"\n    },\n    \"cfdFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a contract for difference order\",\n      \"default\": false\n    },\n    \"locateBroker\": {\n      \"type\": \"string\",\n      \"description\": \"Locate broker for short sell orders\"\n    },\n    \"locateId\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Locate ID for short sell orders\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the order was created\"\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last order update\"\n    },\n    \"routes\": {\n      \"type\": \"array\",\n      \"description\": \"Routes associated with this order\",\n      \"items\": {\n        \"$ref\": \"https://bloomberg.com/schemas/trade.json\"\n      }\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/order.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Order
---
