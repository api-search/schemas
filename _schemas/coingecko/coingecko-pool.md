---
description: A decentralized exchange liquidity pool as represented in the CoinGecko Onchain DEX API, including trading pair information, price data, volume, and liquidity metrics.
layout: schema
name: CoinGecko Onchain Liquidity Pool
properties_list:
- description: Pool identifier in network_address format (e.g., eth_0x1234...)
  name: id
  type: string
- description: Resource type identifier
  name: type
  type: string
- description: Pool attributes containing market and metadata
  name: attributes
  type: object
- description: Related resource references
  name: relationships
  type: object
provider_name: CoinGecko
provider_slug: coingecko
schema_file: json-schema/coingecko-pool-schema.json
slug: coingecko-pool
source_filename: coingecko-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/coingecko/pool.json\",\n  \"title\": \"CoinGecko Onchain Liquidity Pool\",\n  \"description\": \"A decentralized exchange liquidity pool as represented in the CoinGecko Onchain DEX API, including trading pair information, price data, volume, and liquidity metrics.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Pool identifier in network_address format (e.g., eth_0x1234...)\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"pool\",\n      \"description\": \"Resource type identifier\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Pool attributes containing market and metadata\",\n      \"properties\": {\n        \"base_token_price_usd\": {\n          \"type\": [\"string\", \"null\"],\n    \
  \      \"description\": \"Base token price in USD\"\n        },\n        \"base_token_price_native_currency\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Base token price in the network native currency\"\n        },\n        \"quote_token_price_usd\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Quote token price in USD\"\n        },\n        \"quote_token_price_native_currency\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Quote token price in network native currency\"\n        },\n        \"base_token_price_quote_token\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Base token price denominated in the quote token\"\n        },\n        \"quote_token_price_base_token\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Quote token price denominated in the base token\"\n        },\n        \"address\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Pool smart contract address\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Pool name (typically BASE / QUOTE format)\"\n        },\n        \"pool_created_at\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the pool was created\"\n        },\n        \"fdv_usd\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Fully diluted valuation of the base token in USD\"\n        },\n        \"market_cap_usd\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Market capitalization of the base token in USD\"\n        },\n        \"price_change_percentage\": {\n          \"type\": \"object\",\n          \"description\": \"Price change percentages over various timeframes\",\n          \"properties\": {\n            \"m5\": {\n              \"type\": [\"string\", \"null\"],\n    \
  \          \"description\": \"5-minute price change percentage\"\n            },\n            \"h1\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"1-hour price change percentage\"\n            },\n            \"h6\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"6-hour price change percentage\"\n            },\n            \"h24\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"24-hour price change percentage\"\n            }\n          }\n        },\n        \"transactions\": {\n          \"type\": \"object\",\n          \"description\": \"Transaction counts grouped by timeframe\",\n          \"properties\": {\n            \"m5\": { \"$ref\": \"#/$defs/TransactionCount\" },\n            \"m15\": { \"$ref\": \"#/$defs/TransactionCount\" },\n            \"m30\": { \"$ref\": \"#/$defs/TransactionCount\" },\n            \"h1\": { \"$ref\": \"#/$defs/TransactionCount\" },\n\
  \            \"h24\": { \"$ref\": \"#/$defs/TransactionCount\" }\n          }\n        },\n        \"volume_usd\": {\n          \"type\": \"object\",\n          \"description\": \"Trading volume in USD over various timeframes\",\n          \"properties\": {\n            \"m5\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"5-minute volume in USD\"\n            },\n            \"h1\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"1-hour volume in USD\"\n            },\n            \"h6\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"6-hour volume in USD\"\n            },\n            \"h24\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"24-hour volume in USD\"\n            }\n          }\n        },\n        \"reserve_in_usd\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Total liquidity reserve in the\
  \ pool in USD\"\n        }\n      }\n    },\n    \"relationships\": {\n      \"type\": \"object\",\n      \"description\": \"Related resource references\",\n      \"properties\": {\n        \"base_token\": {\n          \"$ref\": \"#/$defs/Relationship\"\n        },\n        \"quote_token\": {\n          \"$ref\": \"#/$defs/Relationship\"\n        },\n        \"dex\": {\n          \"$ref\": \"#/$defs/Relationship\"\n        },\n        \"network\": {\n          \"$ref\": \"#/$defs/Relationship\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"TransactionCount\": {\n      \"type\": \"object\",\n      \"description\": \"Transaction count breakdown for a timeframe\",\n      \"properties\": {\n        \"buys\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of buy transactions\",\n          \"minimum\": 0\n        },\n        \"sells\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of sell transactions\",\n          \"minimum\": 0\n\
  \        },\n        \"buyers\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of unique buyer addresses\",\n          \"minimum\": 0\n        },\n        \"sellers\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of unique seller addresses\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"Relationship\": {\n      \"type\": \"object\",\n      \"description\": \"JSON:API relationship reference to a related resource\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"Related resource identifier\"\n            },\n            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"Related resource type\"\n            }\n          },\n          \"required\": [\"id\", \"type\"]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/coingecko/refs/heads/main/json-schema/coingecko-pool-schema.json
tags:
- Aggregator
- Blockchain
- Cryptocurrency
- Decentralized Exchanges
- DeFi
- DEX
- Exchanges
- Liquidity Pools
- Market Data
- NFTs
- Onchain Data
- Prices
title: CoinGecko Onchain Liquidity Pool
---
