---
description: Represents a trading order on the Binance exchange, applicable across spot, margin, and futures markets.
layout: schema
name: Binance Order
properties_list:
- description: Trading pair symbol, e.g. BTCUSDT.
  name: symbol
  type: string
- description: Unique order identifier assigned by Binance.
  name: orderId
  type: integer
- description: Order list identifier for OCO orders. -1 if not part of an OCO.
  name: orderListId
  type: integer
- description: Client-specified unique order identifier.
  name: clientOrderId
  type: string
- description: Order price as a decimal string.
  name: price
  type: string
- description: Original order quantity.
  name: origQty
  type: string
- description: Quantity that has been executed/filled.
  name: executedQty
  type: string
- description: Cumulative quote asset quantity transacted.
  name: cummulativeQuoteQty
  type: string
- description: Current order status.
  name: status
  type: string
- description: Time in force policy.
  name: timeInForce
  type: string
- description: Order type.
  name: type
  type: string
- description: 'Order side: buy or sell.'
  name: side
  type: string
- description: Stop/trigger price for conditional orders.
  name: stopPrice
  type: string
- description: Iceberg quantity for iceberg orders.
  name: icebergQty
  type: string
- description: Order creation time in milliseconds since Unix epoch.
  name: time
  type: integer
- description: Last update time in milliseconds since Unix epoch.
  name: updateTime
  type: integer
- description: Whether the order is currently on the order book.
  name: isWorking
  type: boolean
- description: Time when the order started working on the book.
  name: workingTime
  type: integer
- description: Original quote order quantity for market orders.
  name: origQuoteOrderQty
  type: string
- description: Self-trade prevention mode.
  name: selfTradePreventionMode
  type: string
- description: Position side for futures hedge mode.
  name: positionSide
  type: string
- description: Whether this is a reduce-only order (futures).
  name: reduceOnly
  type: boolean
- description: Whether this order closes the entire position (futures).
  name: closePosition
  type: boolean
- description: Activation price for trailing stop market orders.
  name: activatePrice
  type: string
- description: Callback rate for trailing stop market orders.
  name: priceRate
  type: string
- description: Stop price trigger type for futures.
  name: workingType
  type: string
- description: Whether price protection is enabled.
  name: priceProtect
  type: boolean
provider_name: Binance
provider_slug: binance
schema_file: json-schema/binance-order-schema.json
slug: binance-order
source_filename: binance-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/binance/order.json\",\n  \"title\": \"Binance Order\",\n  \"description\": \"Represents a trading order on the Binance exchange, applicable across spot, margin, and futures markets.\",\n  \"type\": \"object\",\n  \"required\": [\"symbol\", \"side\", \"type\"],\n  \"properties\": {\n    \"symbol\": {\n      \"type\": \"string\",\n      \"description\": \"Trading pair symbol, e.g. BTCUSDT.\",\n      \"pattern\": \"^[A-Z0-9]+$\"\n    },\n    \"orderId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unique order identifier assigned by Binance.\"\n    },\n    \"orderListId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Order list identifier for OCO orders. -1 if not part of an OCO.\"\n    },\n    \"clientOrderId\": {\n      \"type\": \"string\",\n      \"description\": \"Client-specified\
  \ unique order identifier.\",\n      \"maxLength\": 36\n    },\n    \"price\": {\n      \"type\": \"string\",\n      \"description\": \"Order price as a decimal string.\",\n      \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"origQty\": {\n      \"type\": \"string\",\n      \"description\": \"Original order quantity.\",\n      \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"executedQty\": {\n      \"type\": \"string\",\n      \"description\": \"Quantity that has been executed/filled.\",\n      \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"cummulativeQuoteQty\": {\n      \"type\": \"string\",\n      \"description\": \"Cumulative quote asset quantity transacted.\",\n      \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current order status.\",\n      \"enum\": [\n        \"NEW\",\n        \"PARTIALLY_FILLED\",\n        \"FILLED\",\n        \"CANCELED\",\n        \"PENDING_CANCEL\",\n        \"REJECTED\"\
  ,\n        \"EXPIRED\",\n        \"EXPIRED_IN_MATCH\"\n      ]\n    },\n    \"timeInForce\": {\n      \"type\": \"string\",\n      \"description\": \"Time in force policy.\",\n      \"enum\": [\"GTC\", \"IOC\", \"FOK\", \"GTX\", \"GTD\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Order type.\",\n      \"enum\": [\n        \"LIMIT\",\n        \"MARKET\",\n        \"STOP_LOSS\",\n        \"STOP_LOSS_LIMIT\",\n        \"TAKE_PROFIT\",\n        \"TAKE_PROFIT_LIMIT\",\n        \"LIMIT_MAKER\",\n        \"STOP\",\n        \"STOP_MARKET\",\n        \"TAKE_PROFIT_MARKET\",\n        \"TRAILING_STOP_MARKET\"\n      ]\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"description\": \"Order side: buy or sell.\",\n      \"enum\": [\"BUY\", \"SELL\"]\n    },\n    \"stopPrice\": {\n      \"type\": \"string\",\n      \"description\": \"Stop/trigger price for conditional orders.\",\n      \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"icebergQty\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Iceberg quantity for iceberg orders.\",\n      \"pattern\": \"^\\\\d+\\\\.?\\\\d*$\"\n    },\n    \"time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Order creation time in milliseconds since Unix epoch.\"\n    },\n    \"updateTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Last update time in milliseconds since Unix epoch.\"\n    },\n    \"isWorking\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the order is currently on the order book.\"\n    },\n    \"workingTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Time when the order started working on the book.\"\n    },\n    \"origQuoteOrderQty\": {\n      \"type\": \"string\",\n      \"description\": \"Original quote order quantity for market orders.\"\n    },\n    \"selfTradePreventionMode\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Self-trade prevention mode.\",\n      \"enum\": [\"EXPIRE_TAKER\", \"EXPIRE_MAKER\", \"EXPIRE_BOTH\", \"NONE\"]\n    },\n    \"positionSide\": {\n      \"type\": \"string\",\n      \"description\": \"Position side for futures hedge mode.\",\n      \"enum\": [\"BOTH\", \"LONG\", \"SHORT\"]\n    },\n    \"reduceOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a reduce-only order (futures).\"\n    },\n    \"closePosition\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this order closes the entire position (futures).\"\n    },\n    \"activatePrice\": {\n      \"type\": \"string\",\n      \"description\": \"Activation price for trailing stop market orders.\"\n    },\n    \"priceRate\": {\n      \"type\": \"string\",\n      \"description\": \"Callback rate for trailing stop market orders.\"\n    },\n    \"workingType\": {\n      \"type\": \"string\",\n      \"description\": \"Stop price trigger type for futures.\"\
  ,\n      \"enum\": [\"MARK_PRICE\", \"CONTRACT_PRICE\"]\n    },\n    \"priceProtect\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether price protection is enabled.\"\n    }\n  },\n  \"$defs\": {\n    \"Fill\": {\n      \"type\": \"object\",\n      \"description\": \"A trade fill executed against this order.\",\n      \"properties\": {\n        \"price\": {\n          \"type\": \"string\",\n          \"description\": \"Fill execution price.\"\n        },\n        \"qty\": {\n          \"type\": \"string\",\n          \"description\": \"Fill quantity.\"\n        },\n        \"commission\": {\n          \"type\": \"string\",\n          \"description\": \"Commission charged for this fill.\"\n        },\n        \"commissionAsset\": {\n          \"type\": \"string\",\n          \"description\": \"Asset used for commission payment.\"\n        },\n        \"tradeId\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Trade ID\
  \ for this fill.\"\n        }\n      },\n      \"required\": [\"price\", \"qty\", \"commission\", \"commissionAsset\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/binance/refs/heads/main/json-schema/binance-order-schema.json
tags:
- Cryptocurrency
- Exchange
- Trading
- Blockchain
- Finance
- DeFi
- Market Data
title: Binance Order
---
