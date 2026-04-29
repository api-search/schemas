---
description: A cryptocurrency coin as represented in the CoinGecko API, including market data, metadata, and platform contract addresses.
layout: schema
name: CoinGecko Coin
properties_list:
- description: Unique CoinGecko identifier for the coin (e.g., bitcoin, ethereum)
  name: id
  type: string
- description: Coin ticker symbol (e.g., btc, eth)
  name: symbol
  type: string
- description: Display name of the coin (e.g., Bitcoin, Ethereum)
  name: name
  type: string
- description: Asset platform identifier if the coin is a token on another platform
  name: asset_platform_id
  type:
  - string
  - 'null'
- description: Map of platform names to contract addresses
  name: platforms
  type: object
- description: Average block time in minutes for the coin's blockchain
  name: block_time_in_minutes
  type: integer
- description: Mining or consensus hashing algorithm used
  name: hashing_algorithm
  type:
  - string
  - 'null'
- description: Categories the coin belongs to (e.g., Cryptocurrency, Smart Contract Platform)
  name: categories
  type: array
- description: Localized descriptions of the coin
  name: description
  type: object
- description: ''
  name: links
  type: object
- description: ''
  name: image
  type: object
- description: Date the coin was created or launched
  name: genesis_date
  type:
  - string
  - 'null'
- description: Current market capitalization ranking position
  name: market_cap_rank
  type:
  - integer
  - 'null'
- description: ''
  name: market_data
  type: object
- description: ''
  name: community_data
  type: object
- description: ''
  name: developer_data
  type: object
- description: Timestamp of the last data update
  name: last_updated
  type: string
provider_name: CoinGecko
provider_slug: coingecko
schema_file: json-schema/coingecko-coin-schema.json
slug: coingecko-coin
source_filename: coingecko-coin-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/coingecko/coin.json\",\n  \"title\": \"CoinGecko Coin\",\n  \"description\": \"A cryptocurrency coin as represented in the CoinGecko API, including market data, metadata, and platform contract addresses.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"symbol\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique CoinGecko identifier for the coin (e.g., bitcoin, ethereum)\"\n    },\n    \"symbol\": {\n      \"type\": \"string\",\n      \"description\": \"Coin ticker symbol (e.g., btc, eth)\",\n      \"minLength\": 1\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the coin (e.g., Bitcoin, Ethereum)\",\n      \"minLength\": 1\n    },\n    \"asset_platform_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Asset platform identifier\
  \ if the coin is a token on another platform\"\n    },\n    \"platforms\": {\n      \"type\": \"object\",\n      \"description\": \"Map of platform names to contract addresses\",\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"description\": \"Contract address on the platform\"\n      }\n    },\n    \"block_time_in_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Average block time in minutes for the coin's blockchain\",\n      \"minimum\": 0\n    },\n    \"hashing_algorithm\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Mining or consensus hashing algorithm used\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Categories the coin belongs to (e.g., Cryptocurrency, Smart Contract Platform)\"\n    },\n    \"description\": {\n      \"type\": \"object\",\n      \"description\": \"Localized descriptions of the coin\",\n \
  \     \"properties\": {\n        \"en\": {\n          \"type\": \"string\",\n          \"description\": \"English language description\"\n        }\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"links\": {\n      \"$ref\": \"#/$defs/CoinLinks\"\n    },\n    \"image\": {\n      \"$ref\": \"#/$defs/ImageSet\"\n    },\n    \"genesis_date\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date the coin was created or launched\"\n    },\n    \"market_cap_rank\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Current market capitalization ranking position\",\n      \"minimum\": 1\n    },\n    \"market_data\": {\n      \"$ref\": \"#/$defs/MarketData\"\n    },\n    \"community_data\": {\n      \"$ref\": \"#/$defs/CommunityData\"\n    },\n    \"developer_data\": {\n      \"$ref\": \"#/$defs/DeveloperData\"\n    },\n    \"last_updated\": {\n      \"type\": \"string\",\n  \
  \    \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last data update\"\n    }\n  },\n  \"$defs\": {\n    \"CoinLinks\": {\n      \"type\": \"object\",\n      \"description\": \"Links to official and community resources for the coin\",\n      \"properties\": {\n        \"homepage\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"description\": \"Official homepage URLs\"\n        },\n        \"blockchain_site\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Blockchain explorer URLs\"\n        },\n        \"official_forum_url\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Official forum URLs\"\n        },\n        \"chat_url\": {\n          \"type\": \"array\",\n          \"items\":\
  \ {\n            \"type\": \"string\"\n          },\n          \"description\": \"Chat platform URLs (Discord, Telegram, etc.)\"\n        },\n        \"announcement_url\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Announcement and blog URLs\"\n        },\n        \"twitter_screen_name\": {\n          \"type\": \"string\",\n          \"description\": \"Twitter/X handle\"\n        },\n        \"facebook_username\": {\n          \"type\": \"string\",\n          \"description\": \"Facebook page username\"\n        },\n        \"telegram_channel_identifier\": {\n          \"type\": \"string\",\n          \"description\": \"Telegram channel identifier\"\n        },\n        \"subreddit_url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"Reddit subreddit URL\"\n        },\n        \"repos_url\": {\n          \"type\": \"object\",\n     \
  \     \"properties\": {\n            \"github\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\",\n                \"format\": \"uri\"\n              },\n              \"description\": \"GitHub repository URLs\"\n            },\n            \"bitbucket\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\",\n                \"format\": \"uri\"\n              },\n              \"description\": \"Bitbucket repository URLs\"\n            }\n          },\n          \"description\": \"Source code repository URLs\"\n        }\n      }\n    },\n    \"ImageSet\": {\n      \"type\": \"object\",\n      \"description\": \"Coin logo images at various sizes\",\n      \"properties\": {\n        \"thumb\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Thumbnail image URL\"\n        },\n        \"small\": {\n          \"type\": \"string\",\n   \
  \       \"format\": \"uri\",\n          \"description\": \"Small image URL\"\n        },\n        \"large\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Large image URL\"\n        }\n      }\n    },\n    \"MarketData\": {\n      \"type\": \"object\",\n      \"description\": \"Current market data for the coin across multiple currencies\",\n      \"properties\": {\n        \"current_price\": {\n          \"type\": \"object\",\n          \"description\": \"Current price in various currencies\",\n          \"additionalProperties\": {\n            \"type\": \"number\"\n          }\n        },\n        \"market_cap\": {\n          \"type\": \"object\",\n          \"description\": \"Market capitalization in various currencies\",\n          \"additionalProperties\": {\n            \"type\": \"number\"\n          }\n        },\n        \"total_volume\": {\n          \"type\": \"object\",\n          \"description\": \"24-hour trading volume in\
  \ various currencies\",\n          \"additionalProperties\": {\n            \"type\": \"number\"\n          }\n        },\n        \"high_24h\": {\n          \"type\": \"object\",\n          \"description\": \"24-hour high price in various currencies\",\n          \"additionalProperties\": {\n            \"type\": \"number\"\n          }\n        },\n        \"low_24h\": {\n          \"type\": \"object\",\n          \"description\": \"24-hour low price in various currencies\",\n          \"additionalProperties\": {\n            \"type\": \"number\"\n          }\n        },\n        \"price_change_24h\": {\n          \"type\": \"number\",\n          \"description\": \"24-hour price change in USD\"\n        },\n        \"price_change_percentage_24h\": {\n          \"type\": \"number\",\n          \"description\": \"24-hour price change percentage\"\n        },\n        \"price_change_percentage_7d\": {\n          \"type\": \"number\",\n          \"description\": \"7-day price change percentage\"\
  \n        },\n        \"price_change_percentage_14d\": {\n          \"type\": \"number\",\n          \"description\": \"14-day price change percentage\"\n        },\n        \"price_change_percentage_30d\": {\n          \"type\": \"number\",\n          \"description\": \"30-day price change percentage\"\n        },\n        \"price_change_percentage_60d\": {\n          \"type\": \"number\",\n          \"description\": \"60-day price change percentage\"\n        },\n        \"price_change_percentage_200d\": {\n          \"type\": \"number\",\n          \"description\": \"200-day price change percentage\"\n        },\n        \"price_change_percentage_1y\": {\n          \"type\": \"number\",\n          \"description\": \"1-year price change percentage\"\n        },\n        \"market_cap_change_24h\": {\n          \"type\": \"number\",\n          \"description\": \"24-hour market cap change in USD\"\n        },\n        \"market_cap_change_percentage_24h\": {\n          \"type\": \"number\"\
  ,\n          \"description\": \"24-hour market cap change percentage\"\n        },\n        \"circulating_supply\": {\n          \"type\": \"number\",\n          \"description\": \"Current circulating supply\"\n        },\n        \"total_supply\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Total supply (null if not applicable)\"\n        },\n        \"max_supply\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Maximum supply (null if unlimited)\"\n        },\n        \"ath\": {\n          \"type\": \"object\",\n          \"description\": \"All-time high price in various currencies\",\n          \"additionalProperties\": {\n            \"type\": \"number\"\n          }\n        },\n        \"ath_change_percentage\": {\n          \"type\": \"object\",\n          \"description\": \"Percentage change from all-time high\",\n          \"additionalProperties\": {\n            \"type\": \"number\"\n          }\n        },\n    \
  \    \"ath_date\": {\n          \"type\": \"object\",\n          \"description\": \"Date of all-time high in various currencies\",\n          \"additionalProperties\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        },\n        \"atl\": {\n          \"type\": \"object\",\n          \"description\": \"All-time low price in various currencies\",\n          \"additionalProperties\": {\n            \"type\": \"number\"\n          }\n        },\n        \"atl_change_percentage\": {\n          \"type\": \"object\",\n          \"description\": \"Percentage change from all-time low\",\n          \"additionalProperties\": {\n            \"type\": \"number\"\n          }\n        },\n        \"atl_date\": {\n          \"type\": \"object\",\n          \"description\": \"Date of all-time low in various currencies\",\n          \"additionalProperties\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n      \
  \  },\n        \"total_value_locked\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Total value locked in DeFi protocols\"\n        },\n        \"fully_diluted_valuation\": {\n          \"type\": \"object\",\n          \"description\": \"Fully diluted valuation in various currencies\",\n          \"additionalProperties\": {\n            \"type\": \"number\"\n          }\n        },\n        \"last_updated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp of the last market data update\"\n        }\n      }\n    },\n    \"CommunityData\": {\n      \"type\": \"object\",\n      \"description\": \"Community engagement metrics for the coin\",\n      \"properties\": {\n        \"facebook_likes\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Number of Facebook page likes\"\n        },\n        \"twitter_followers\": {\n          \"type\": [\"integer\", \"null\"],\n\
  \          \"description\": \"Number of Twitter/X followers\"\n        },\n        \"reddit_average_posts_48h\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Average Reddit posts in 48 hours\"\n        },\n        \"reddit_average_comments_48h\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Average Reddit comments in 48 hours\"\n        },\n        \"reddit_subscribers\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Number of Reddit subscribers\"\n        },\n        \"reddit_accounts_active_48h\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Active Reddit accounts in 48 hours\"\n        },\n        \"telegram_channel_user_count\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Number of Telegram channel users\"\n        }\n      }\n    },\n    \"DeveloperData\": {\n      \"type\": \"object\",\n      \"description\": \"Developer\
  \ activity metrics from source code repositories\",\n      \"properties\": {\n        \"forks\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Number of repository forks\"\n        },\n        \"stars\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Number of repository stars\"\n        },\n        \"subscribers\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Number of repository watchers\"\n        },\n        \"total_issues\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Total number of issues\"\n        },\n        \"closed_issues\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Number of closed issues\"\n        },\n        \"pull_requests_merged\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Number of merged pull requests\"\n        },\n        \"pull_request_contributors\": {\n         \
  \ \"type\": [\"integer\", \"null\"],\n          \"description\": \"Number of pull request contributors\"\n        },\n        \"commit_count_4_weeks\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Number of commits in the last 4 weeks\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/coingecko/refs/heads/main/json-schema/coingecko-coin-schema.json
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
title: CoinGecko Coin
---
