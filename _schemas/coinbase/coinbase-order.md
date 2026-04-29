---
description: A trading order on the Coinbase platform, applicable across Advanced Trade, Exchange, and Prime APIs. Represents a request to buy or sell a cryptocurrency at a specified price and quantity.
layout: schema
name: Coinbase Order
properties_list:
- description: Unique identifier for the order assigned by Coinbase
  name: order_id
  type: string
- description: Client-specified unique identifier for the order
  name: client_order_id
  type: string
- description: Trading pair identifier such as BTC-USD
  name: product_id
  type: string
- description: Whether this is a buy or sell order
  name: side
  type: string
- description: Type of order determining execution behavior
  name: order_type
  type: string
- description: Current lifecycle status of the order
  name: status
  type: string
- description: Time-in-force policy governing how long the order remains active
  name: time_in_force
  type: string
- description: Quantity of base currency to trade
  name: base_size
  type: string
- description: Quantity of quote currency to spend or receive
  name: quote_size
  type: string
- description: Limit price for limit and stop-limit orders
  name: limit_price
  type: string
- description: Trigger price for stop and stop-limit orders
  name: stop_price
  type: string
- description: Amount that has been filled so far
  name: filled_size
  type: string
- description: Total value of filled portion in quote currency
  name: filled_value
  type: string
- description: Volume-weighted average price of fills
  name: average_filled_price
  type: string
- description: Total fees charged for the order
  name: total_fees
  type: string
- description: Number of individual fills for the order
  name: number_of_fills
  type: integer
- description: Percentage of the order that has been filled
  name: completion_percentage
  type: string
- description: Portfolio that owns the order (Prime and Advanced Trade)
  name: portfolio_id
  type: string
- description: ISO 8601 timestamp when the order was created
  name: created_at
  type: string
- description: ISO 8601 timestamp when the order was completed
  name: completed_at
  type: string
- description: ISO 8601 timestamp when the order expires
  name: expiry_time
  type: string
- description: Whether the order is post-only (maker only)
  name: post_only
  type: boolean
provider_name: Coinbase
provider_slug: coinbase
schema_file: json-schema/coinbase-order-schema.json
slug: coinbase-order
source_filename: coinbase-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://coinbase.com/schemas/coinbase/order.json\",\n  \"title\": \"Coinbase Order\",\n  \"description\": \"A trading order on the Coinbase platform, applicable across Advanced Trade, Exchange, and Prime APIs. Represents a request to buy or sell a cryptocurrency at a specified price and quantity.\",\n  \"type\": \"object\",\n  \"required\": [\"product_id\", \"side\", \"order_type\"],\n  \"properties\": {\n    \"order_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the order assigned by Coinbase\"\n    },\n    \"client_order_id\": {\n      \"type\": \"string\",\n      \"description\": \"Client-specified unique identifier for the order\"\n    },\n    \"product_id\": {\n      \"type\": \"string\",\n      \"description\": \"Trading pair identifier such as BTC-USD\",\n      \"pattern\": \"^[A-Z0-9]+-[A-Z0-9]+$\"\n    },\n    \"side\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Whether this is a buy or sell order\",\n      \"enum\": [\"BUY\", \"SELL\"]\n    },\n    \"order_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of order determining execution behavior\",\n      \"enum\": [\"MARKET\", \"LIMIT\", \"STOP\", \"STOP_LIMIT\", \"TWAP\", \"BLOCK\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the order\",\n      \"enum\": [\"OPEN\", \"PENDING\", \"FILLED\", \"CANCELLED\", \"EXPIRED\", \"FAILED\"]\n    },\n    \"time_in_force\": {\n      \"type\": \"string\",\n      \"description\": \"Time-in-force policy governing how long the order remains active\",\n      \"enum\": [\"GOOD_UNTIL_CANCELLED\", \"GOOD_UNTIL_DATE\", \"IMMEDIATE_OR_CANCEL\", \"FILL_OR_KILL\"]\n    },\n    \"base_size\": {\n      \"type\": \"string\",\n      \"description\": \"Quantity of base currency to trade\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"quote_size\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Quantity of quote currency to spend or receive\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"limit_price\": {\n      \"type\": \"string\",\n      \"description\": \"Limit price for limit and stop-limit orders\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"stop_price\": {\n      \"type\": \"string\",\n      \"description\": \"Trigger price for stop and stop-limit orders\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"filled_size\": {\n      \"type\": \"string\",\n      \"description\": \"Amount that has been filled so far\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"filled_value\": {\n      \"type\": \"string\",\n      \"description\": \"Total value of filled portion in quote currency\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"average_filled_price\": {\n      \"type\": \"string\",\n      \"description\": \"Volume-weighted average price\
  \ of fills\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"total_fees\": {\n      \"type\": \"string\",\n      \"description\": \"Total fees charged for the order\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"number_of_fills\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of individual fills for the order\",\n      \"minimum\": 0\n    },\n    \"completion_percentage\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage of the order that has been filled\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"portfolio_id\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio that owns the order (Prime and Advanced Trade)\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the order was created\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"\
  description\": \"ISO 8601 timestamp when the order was completed\"\n    },\n    \"expiry_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the order expires\"\n    },\n    \"post_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the order is post-only (maker only)\"\n    }\n  },\n  \"$defs\": {\n    \"Fill\": {\n      \"type\": \"object\",\n      \"description\": \"An individual fill representing partial or full execution of an order\",\n      \"required\": [\"trade_id\", \"price\", \"size\"],\n      \"properties\": {\n        \"trade_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique trade identifier\"\n        },\n        \"entry_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique fill entry identifier\"\n        },\n        \"order_id\": {\n          \"type\": \"string\",\n          \"description\": \"Order that generated this fill\"\n\
  \        },\n        \"product_id\": {\n          \"type\": \"string\",\n          \"description\": \"Product traded\"\n        },\n        \"price\": {\n          \"type\": \"string\",\n          \"description\": \"Execution price\"\n        },\n        \"size\": {\n          \"type\": \"string\",\n          \"description\": \"Fill size\"\n        },\n        \"commission\": {\n          \"type\": \"string\",\n          \"description\": \"Fee charged for this fill\"\n        },\n        \"side\": {\n          \"type\": \"string\",\n          \"description\": \"Trade side\",\n          \"enum\": [\"BUY\", \"SELL\"]\n        },\n        \"liquidity\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the fill was maker or taker\",\n          \"enum\": [\"M\", \"T\"]\n        },\n        \"trade_time\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the trade occurred\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/json-schema/coinbase-order-schema.json
tags:
- Blockchain
- Cryptocurrency
- Custody
- Exchange
- Onramp
- Payments
- Trading
- Wallet
- Web3
title: Coinbase Order
---
