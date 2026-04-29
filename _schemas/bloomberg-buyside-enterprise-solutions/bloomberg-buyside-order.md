---
description: A trading order representing an instruction to buy or sell a financial instrument, supporting various order types, time-in-force options, and algorithmic execution strategies for institutional buy-side trading.
layout: schema
name: Bloomberg Buyside Order
properties_list:
- description: Unique order identifier
  name: id
  type: string
- description: Bloomberg security identifier (e.g., 'AAPL US Equity')
  name: security
  type: string
- description: Human-readable security name
  name: securityName
  type: string
- description: Order side indicating the direction of the trade
  name: side
  type: string
- description: Order type determining execution behavior
  name: orderType
  type: string
- description: Total order quantity in shares or units
  name: quantity
  type: number
- description: Cumulative filled quantity
  name: filledQuantity
  type: number
- description: Remaining quantity to be filled
  name: remainingQuantity
  type: number
- description: Limit price for LIMIT and STOP_LIMIT orders
  name: limitPrice
  type: number
- description: Stop trigger price for STOP and STOP_LIMIT orders
  name: stopPrice
  type: number
- description: Volume-weighted average price of all fills
  name: averageFillPrice
  type: number
- description: Current order lifecycle status
  name: status
  type: string
- description: Time-in-force instruction governing order duration
  name: timeInForce
  type: string
- description: Expiration date for Good-Till-Date (GTD) orders
  name: expirationDate
  type: string
- description: Target portfolio for post-trade allocation
  name: portfolioId
  type: string
- description: Broker identifier for order routing
  name: brokerId
  type: string
- description: Algorithmic execution strategy name
  name: algorithm
  type: string
- description: Algorithm-specific execution parameters
  name: algorithmParams
  type: object
- description: Order currency (ISO 4217)
  name: currency
  type: string
- description: Identifier of the trader who placed the order
  name: trader
  type: string
- description: Execution reports (fills) for this order
  name: executions
  type: array
- description: Order creation timestamp
  name: createdAt
  type: string
- description: Most recent order update timestamp
  name: updatedAt
  type: string
provider_name: Bloomberg Buyside Enterprise Solutions
provider_slug: bloomberg-buyside-enterprise-solutions
schema_file: json-schema/bloomberg-buyside-order-schema.json
slug: bloomberg-buyside-order
source_filename: bloomberg-buyside-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.bloomberg.com/schemas/buyside/order.json\",\n  \"title\": \"Bloomberg Buyside Order\",\n  \"description\": \"A trading order representing an instruction to buy or sell a financial instrument, supporting various order types, time-in-force options, and algorithmic execution strategies for institutional buy-side trading.\",\n  \"type\": \"object\",\n  \"required\": [\"security\", \"side\", \"orderType\", \"quantity\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique order identifier\"\n    },\n    \"security\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg security identifier (e.g., 'AAPL US Equity')\"\n    },\n    \"securityName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable security name\"\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"enum\": [\"BUY\", \"SELL\", \"SHORT_SELL\"\
  , \"BUY_TO_COVER\"],\n      \"description\": \"Order side indicating the direction of the trade\"\n    },\n    \"orderType\": {\n      \"type\": \"string\",\n      \"enum\": [\"MARKET\", \"LIMIT\", \"STOP\", \"STOP_LIMIT\", \"PEGGED\", \"VWAP\", \"TWAP\"],\n      \"description\": \"Order type determining execution behavior\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"exclusiveMinimum\": true,\n      \"description\": \"Total order quantity in shares or units\"\n    },\n    \"filledQuantity\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Cumulative filled quantity\"\n    },\n    \"remainingQuantity\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Remaining quantity to be filled\"\n    },\n    \"limitPrice\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Limit price for LIMIT and STOP_LIMIT orders\"\n    },\n    \"stopPrice\": {\n      \"type\"\
  : \"number\",\n      \"minimum\": 0,\n      \"description\": \"Stop trigger price for STOP and STOP_LIMIT orders\"\n    },\n    \"averageFillPrice\": {\n      \"type\": \"number\",\n      \"description\": \"Volume-weighted average price of all fills\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"NEW\", \"PENDING\", \"PARTIALLY_FILLED\", \"FILLED\", \"CANCELLED\", \"REJECTED\", \"EXPIRED\"],\n      \"description\": \"Current order lifecycle status\"\n    },\n    \"timeInForce\": {\n      \"type\": \"string\",\n      \"enum\": [\"DAY\", \"GTC\", \"IOC\", \"FOK\", \"GTD\"],\n      \"description\": \"Time-in-force instruction governing order duration\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Expiration date for Good-Till-Date (GTD) orders\"\n    },\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"Target portfolio for post-trade allocation\"\n    },\n \
  \   \"brokerId\": {\n      \"type\": \"string\",\n      \"description\": \"Broker identifier for order routing\"\n    },\n    \"algorithm\": {\n      \"type\": \"string\",\n      \"description\": \"Algorithmic execution strategy name\"\n    },\n    \"algorithmParams\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Algorithm-specific execution parameters\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Order currency (ISO 4217)\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"trader\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the trader who placed the order\"\n    },\n    \"executions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Execution\"\n      },\n      \"description\": \"Execution reports (fills) for this order\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Order creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Most recent order update timestamp\"\n    }\n  },\n  \"$defs\": {\n    \"Execution\": {\n      \"type\": \"object\",\n      \"description\": \"An execution report representing a partial or complete fill of a trading order\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique execution identifier\"\n        },\n        \"quantity\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"description\": \"Executed quantity\"\n        },\n        \"price\": {\n          \"type\": \"number\",\n          \"description\": \"Execution price\"\n        },\n        \"commission\": {\n          \"type\": \"number\",\n          \"description\": \"Commission charged for this execution\"\n        },\n        \"fees\": {\n          \"type\": \"number\",\n          \"description\"\
  : \"Exchange and regulatory fees\"\n        },\n        \"netAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Net settlement amount\"\n        },\n        \"venue\": {\n          \"type\": \"string\",\n          \"description\": \"Execution venue or exchange\"\n        },\n        \"broker\": {\n          \"type\": \"string\",\n          \"description\": \"Executing broker\"\n        },\n        \"settlementDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Expected settlement date\"\n        },\n        \"executedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Execution timestamp\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-buyside-enterprise-solutions/refs/heads/main/json-schema/bloomberg-buyside-order-schema.json
tags:
- Analytics
- Asset Management
- Buy-Side
- Enterprise Solutions
- Financial Services
- Market Data
- Portfolio Management
- Trading
title: Bloomberg Buyside Order
---
