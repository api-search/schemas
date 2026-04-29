---
description: A trading order in the Bloomberg Execution Management System (EMSX) blotter representing an intent to buy or sell a financial instrument. Orders contain instrument details, quantity, pricing instructions, and lifecycle status, and may have one or more routes to brokers for execution.
layout: schema
name: Bloomberg EMSX Order
properties_list:
- description: EMSX order sequence number, the unique identifier for the order within the blotter
  name: sequenceNumber
  type: integer
- description: Bloomberg security ticker symbol identifying the instrument to trade
  name: ticker
  type: string
- description: Order side indicating the direction of the trade
  name: side
  type: string
- description: Total order quantity in shares, contracts, or face value
  name: amount
  type: number
- description: Order type specifying pricing and execution behavior
  name: orderType
  type: string
- description: Limit price for limit orders (LMT, STP_LMT, LOC)
  name: limitPrice
  type: number
- description: Stop trigger price for stop orders (STP, STP_LMT)
  name: stopPrice
  type: number
- description: Time in force instruction governing how long the order remains active
  name: timeInForce
  type: string
- description: Expiration date for GTD (Good Till Date) orders
  name: goodTillDate
  type: string
- description: Current lifecycle status of the order
  name: status
  type: string
- description: Total quantity filled across all routes
  name: filledAmount
  type: number
- description: Volume-weighted average fill price across all executions
  name: averagePrice
  type: number
- description: Remaining unfilled quantity (amount minus filledAmount)
  name: remainingAmount
  type: number
- description: Asset class of the instrument being traded
  name: assetClass
  type: string
- description: Primary exchange or marketplace for the instrument
  name: exchange
  type: string
- description: Trading currency in ISO 4217 three-letter code
  name: currency
  type: string
- description: Trading account identifier for allocation
  name: account
  type: string
- description: Free-text notes attached to the order by the trader
  name: notes
  type: string
- description: Name of the trader who created the order
  name: traderName
  type: string
- description: ISO 8601 timestamp when the order was created
  name: createdTime
  type: string
- description: ISO 8601 timestamp when the order was last modified
  name: lastModifiedTime
  type: string
- description: Summary of routes associated with this order
  name: routes
  type: array
- description: Custom user-defined fields configured in the EMSX blotter
  name: customFields
  type: object
provider_name: Bloomberg EMSX
provider_slug: bloomberg-emsx
schema_file: json-schema/bloomberg-emsx-order-schema.json
slug: bloomberg-emsx-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.bloomberg.com/schemas/emsx/order.json\",\n  \"title\": \"Bloomberg EMSX Order\",\n  \"description\": \"A trading order in the Bloomberg Execution Management System (EMSX) blotter representing an intent to buy or sell a financial instrument. Orders contain instrument details, quantity, pricing instructions, and lifecycle status, and may have one or more routes to brokers for execution.\",\n  \"type\": \"object\",\n  \"required\": [\"ticker\", \"side\", \"amount\", \"orderType\", \"timeInForce\"],\n  \"properties\": {\n    \"sequenceNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"EMSX order sequence number, the unique identifier for the order within the blotter\"\n    },\n    \"ticker\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg security ticker symbol identifying the instrument to trade\",\n      \"minLength\": 1\n    },\n    \"side\": {\n\
  \      \"type\": \"string\",\n      \"enum\": [\"BUY\", \"SELL\", \"SHORT\", \"COVER\"],\n      \"description\": \"Order side indicating the direction of the trade\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"minimum\": 1,\n      \"description\": \"Total order quantity in shares, contracts, or face value\"\n    },\n    \"orderType\": {\n      \"type\": \"string\",\n      \"enum\": [\"MKT\", \"LMT\", \"STP\", \"STP_LMT\", \"MOC\", \"LOC\", \"VWAP\", \"TWAP\"],\n      \"description\": \"Order type specifying pricing and execution behavior\"\n    },\n    \"limitPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Limit price for limit orders (LMT, STP_LMT, LOC)\"\n    },\n    \"stopPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Stop trigger price for stop orders (STP, STP_LMT)\"\n    },\n    \"timeInForce\": {\n      \"type\": \"string\",\n      \"enum\": [\"DAY\", \"GTC\", \"IOC\", \"FOK\", \"GTD\", \"OPG\", \"CLO\"],\n      \"description\"\
  : \"Time in force instruction governing how long the order remains active\"\n    },\n    \"goodTillDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Expiration date for GTD (Good Till Date) orders\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"NEW\", \"WORKING\", \"PARTIALLY_FILLED\", \"FILLED\", \"CANCELLED\", \"REJECTED\", \"EXPIRED\"],\n      \"description\": \"Current lifecycle status of the order\"\n    },\n    \"filledAmount\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total quantity filled across all routes\"\n    },\n    \"averagePrice\": {\n      \"type\": \"number\",\n      \"description\": \"Volume-weighted average fill price across all executions\"\n    },\n    \"remainingAmount\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Remaining unfilled quantity (amount minus filledAmount)\"\n    },\n    \"assetClass\": {\n      \"type\"\
  : \"string\",\n      \"enum\": [\"Equity\", \"Fixed Income\", \"Futures\", \"Options\", \"FX\"],\n      \"description\": \"Asset class of the instrument being traded\"\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"Primary exchange or marketplace for the instrument\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"Trading currency in ISO 4217 three-letter code\"\n    },\n    \"account\": {\n      \"type\": \"string\",\n      \"description\": \"Trading account identifier for allocation\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Free-text notes attached to the order by the trader\"\n    },\n    \"traderName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the trader who created the order\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp\
  \ when the order was created\"\n    },\n    \"lastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the order was last modified\"\n    },\n    \"routes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RouteSummary\"\n      },\n      \"description\": \"Summary of routes associated with this order\"\n    },\n    \"customFields\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Custom user-defined fields configured in the EMSX blotter\"\n    }\n  },\n  \"$defs\": {\n    \"RouteSummary\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of a route associated with an order\",\n      \"properties\": {\n        \"routeId\": {\n          \"type\": \"integer\",\n          \"description\": \"Route identifier\"\n        },\n        \"broker\": {\n          \"type\": \"string\",\n          \"description\": \"Broker code\"\n\
  \        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"NEW\", \"WORKING\", \"PARTIALLY_FILLED\", \"FILLED\", \"CANCELLED\", \"REJECTED\"],\n          \"description\": \"Route status\"\n        },\n        \"filledAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Quantity filled on this route\"\n        },\n        \"averagePrice\": {\n          \"type\": \"number\",\n          \"description\": \"Average fill price on this route\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-emsx/refs/heads/main/json-schema/bloomberg-emsx-order-schema.json
tags:
- Bloomberg
- Execution Management
- Financial Services
- Order Management
- Trading
title: Bloomberg EMSX Order
---
