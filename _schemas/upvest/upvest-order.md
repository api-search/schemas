---
description: Schema for validating Upvest Investment API order request payloads. Orders represent buy or sell instructions for financial instruments, processed asynchronously with status updates delivered via webhooks.
layout: schema
name: Upvest Order
properties_list:
- description: The unique identifier of the investment account to place the order for.
  name: account_id
  type: string
- description: The unique identifier of the financial instrument to trade.
  name: instrument_id
  type: string
- description: Whether to buy or sell the instrument.
  name: side
  type: string
- description: The order type. MARKET orders execute at the current market price. LIMIT orders execute at or better than the specified limit price. STOP orders become market orders when the stop price is reached.
  name: type
  type: string
- description: The quantity of shares to trade as a decimal string. Either quantity or cash_amount must be provided.
  name: quantity
  type: string
- description: The cash amount to invest as a decimal string. Used for fractional investing. Either quantity or cash_amount must be provided.
  name: cash_amount
  type: string
- description: The limit price as a decimal string. Required for LIMIT orders.
  name: limit_price
  type: string
- description: The stop trigger price as a decimal string. Required for STOP orders.
  name: stop_price
  type: string
- description: The order currency as an ISO 4217 three-letter currency code.
  name: currency
  type: string
provider_name: Upvest
provider_slug: upvest
schema_file: json-schema/upvest-order-schema.json
slug: upvest-order
source_filename: upvest-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://upvest.co/schemas/upvest/order.json\",\n  \"title\": \"Upvest Order\",\n  \"description\": \"Schema for validating Upvest Investment API order request payloads. Orders represent buy or sell instructions for financial instruments, processed asynchronously with status updates delivered via webhooks.\",\n  \"type\": \"object\",\n  \"required\": [\"account_id\", \"instrument_id\", \"side\", \"type\"],\n  \"properties\": {\n    \"account_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the investment account to place the order for.\"\n    },\n    \"instrument_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the financial instrument to trade.\"\n    },\n    \"side\": {\n      \"type\": \"string\",\n      \"enum\": [\"BUY\", \"SELL\"],\n      \"description\"\
  : \"Whether to buy or sell the instrument.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"MARKET\", \"LIMIT\", \"STOP\"],\n      \"description\": \"The order type. MARKET orders execute at the current market price. LIMIT orders execute at or better than the specified limit price. STOP orders become market orders when the stop price is reached.\"\n    },\n    \"quantity\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\",\n      \"description\": \"The quantity of shares to trade as a decimal string. Either quantity or cash_amount must be provided.\"\n    },\n    \"cash_amount\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\",\n      \"description\": \"The cash amount to invest as a decimal string. Used for fractional investing. Either quantity or cash_amount must be provided.\"\n    },\n    \"limit_price\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\",\n      \"description\"\
  : \"The limit price as a decimal string. Required for LIMIT orders.\"\n    },\n    \"stop_price\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\",\n      \"description\": \"The stop trigger price as a decimal string. Required for STOP orders.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"The order currency as an ISO 4217 three-letter currency code.\",\n      \"examples\": [\"EUR\", \"GBP\", \"USD\"]\n    }\n  },\n  \"$defs\": {\n    \"OrderResponse\": {\n      \"type\": \"object\",\n      \"description\": \"The full order object returned by the API after creation or retrieval.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the order.\"\n        },\n        \"account_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\"\
  : \"The account the order belongs to.\"\n        },\n        \"user_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The user who placed the order.\"\n        },\n        \"instrument_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The instrument being traded.\"\n        },\n        \"side\": {\n          \"type\": \"string\",\n          \"enum\": [\"BUY\", \"SELL\"],\n          \"description\": \"Whether this is a buy or sell order.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"MARKET\", \"LIMIT\", \"STOP\"],\n          \"description\": \"The order type.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"NEW\", \"PROCESSING\", \"FILLED\", \"CANCELLED\", \"REJECTED\"],\n          \"description\": \"The current order status.\"\n        },\n        \"quantity\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The order quantity as a decimal string.\"\n        },\n        \"cash_amount\": {\n          \"type\": \"string\",\n          \"description\": \"The cash amount as a decimal string.\"\n        },\n        \"limit_price\": {\n          \"type\": \"string\",\n          \"description\": \"The limit price as a decimal string.\"\n        },\n        \"stop_price\": {\n          \"type\": \"string\",\n          \"description\": \"The stop price as a decimal string.\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\",\n          \"description\": \"The order currency.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the order was placed.\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the order was last updated.\"\
  \n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/upvest/refs/heads/main/json-schema/upvest-order-schema.json
tags:
- Banking Infrastructure
- Fintech
- Investments
- Securities
title: Upvest Order
---
