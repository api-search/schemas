---
description: A trading product representing a cryptocurrency trading pair on Coinbase. Products define the parameters for trading between two currencies including minimum sizes, increments, and trading status.
layout: schema
name: Coinbase Trading Product
properties_list:
- description: Unique identifier for the product, typically formatted as BASE-QUOTE
  name: product_id
  type: string
- description: Base currency code (e.g., BTC)
  name: base_currency
  type: string
- description: Quote currency code (e.g., USD)
  name: quote_currency
  type: string
- description: Minimum order size in base currency
  name: base_min_size
  type: string
- description: Maximum order size in base currency
  name: base_max_size
  type: string
- description: Minimum size increment for orders in base currency
  name: base_increment
  type: string
- description: Minimum order value in quote currency
  name: quote_min_size
  type: string
- description: Maximum order value in quote currency
  name: quote_max_size
  type: string
- description: Minimum price increment in quote currency
  name: quote_increment
  type: string
- description: Human-readable display name for the trading pair
  name: display_name
  type: string
- description: Current trading status of the product
  name: status
  type: string
- description: Type of product
  name: product_type
  type: string
- description: Current price of the product
  name: price
  type: string
- description: 24-hour trading volume in base currency
  name: volume_24h
  type: string
- description: 24-hour price change as a percentage
  name: price_percentage_change_24h
  type: string
- description: Whether margin trading is enabled for this product
  name: margin_enabled
  type: boolean
- description: Whether the product is in post-only mode
  name: post_only
  type: boolean
- description: Whether only limit orders are accepted
  name: limit_only
  type: boolean
- description: Whether only order cancellations are allowed
  name: cancel_only
  type: boolean
- description: Whether trading is completely disabled
  name: trading_disabled
  type: boolean
provider_name: Coinbase
provider_slug: coinbase
schema_file: json-schema/coinbase-product-schema.json
slug: coinbase-product
source_filename: coinbase-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://coinbase.com/schemas/coinbase/product.json\",\n  \"title\": \"Coinbase Trading Product\",\n  \"description\": \"A trading product representing a cryptocurrency trading pair on Coinbase. Products define the parameters for trading between two currencies including minimum sizes, increments, and trading status.\",\n  \"type\": \"object\",\n  \"required\": [\"product_id\", \"base_currency\", \"quote_currency\"],\n  \"properties\": {\n    \"product_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the product, typically formatted as BASE-QUOTE\",\n      \"pattern\": \"^[A-Z0-9]+-[A-Z0-9]+$\"\n    },\n    \"base_currency\": {\n      \"type\": \"string\",\n      \"description\": \"Base currency code (e.g., BTC)\",\n      \"minLength\": 1,\n      \"maxLength\": 10\n    },\n    \"quote_currency\": {\n      \"type\": \"string\",\n      \"description\": \"Quote currency\
  \ code (e.g., USD)\",\n      \"minLength\": 1,\n      \"maxLength\": 10\n    },\n    \"base_min_size\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum order size in base currency\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"base_max_size\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum order size in base currency\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"base_increment\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum size increment for orders in base currency\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"quote_min_size\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum order value in quote currency\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"quote_max_size\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum order value in quote currency\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"quote_increment\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Minimum price increment in quote currency\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the trading pair\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current trading status of the product\",\n      \"enum\": [\"online\", \"offline\", \"delisted\"]\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of product\",\n      \"enum\": [\"SPOT\", \"FUTURE\"]\n    },\n    \"price\": {\n      \"type\": \"string\",\n      \"description\": \"Current price of the product\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"volume_24h\": {\n      \"type\": \"string\",\n      \"description\": \"24-hour trading volume in base currency\",\n      \"pattern\": \"^[0-9]+(\\\\.[0-9]+)?$\"\n    },\n    \"price_percentage_change_24h\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"24-hour price change as a percentage\"\n    },\n    \"margin_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether margin trading is enabled for this product\"\n    },\n    \"post_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the product is in post-only mode\"\n    },\n    \"limit_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether only limit orders are accepted\"\n    },\n    \"cancel_only\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether only order cancellations are allowed\"\n    },\n    \"trading_disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether trading is completely disabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/json-schema/coinbase-product-schema.json
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
title: Coinbase Trading Product
---
