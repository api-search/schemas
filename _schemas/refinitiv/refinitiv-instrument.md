---
description: Represents a financial instrument with its identifiers, pricing data, and metadata as used across Refinitiv Data Platform APIs.
layout: schema
name: Refinitiv Financial Instrument
properties_list:
- description: Reuters Instrument Code (RIC) uniquely identifying the instrument on the Refinitiv platform.
  name: ric
  type: string
- description: International Securities Identification Number (ISIN) for the instrument.
  name: isin
  type:
  - string
  - 'null'
- description: Committee on Uniform Securities Identification Procedures (CUSIP) number.
  name: cusip
  type:
  - string
  - 'null'
- description: Stock Exchange Daily Official List (SEDOL) code.
  name: sedol
  type:
  - string
  - 'null'
- description: Exchange ticker symbol for the instrument.
  name: ticker
  type:
  - string
  - 'null'
- description: Refinitiv Permanent Identifier (PermID) for the instrument.
  name: permId
  type:
  - string
  - 'null'
- description: Legal Entity Identifier (LEI) for the issuing organization.
  name: lei
  type:
  - string
  - 'null'
- description: Human-readable display name of the instrument.
  name: displayName
  type:
  - string
  - 'null'
- description: ISO 4217 currency code for the instrument's trading currency.
  name: currency
  type:
  - string
  - 'null'
- description: Market Identifier Code (MIC) for the exchange where the instrument is traded.
  name: exchangeCode
  type:
  - string
  - 'null'
- description: Human-readable name of the exchange.
  name: exchangeName
  type:
  - string
  - 'null'
- description: The asset class category of the instrument.
  name: assetClass
  type:
  - string
  - 'null'
- description: ISO 3166-1 alpha-2 country code of the primary listing.
  name: country
  type:
  - string
  - 'null'
- description: Current trading status of the instrument.
  name: status
  type:
  - string
  - 'null'
provider_name: Refinitiv
provider_slug: refinitiv
schema_file: json-schema/refinitiv-instrument-schema.json
slug: refinitiv-instrument
source_filename: refinitiv-instrument-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.refinitiv.com/schemas/refinitiv/instrument.json\",\n  \"title\": \"Refinitiv Financial Instrument\",\n  \"description\": \"Represents a financial instrument with its identifiers, pricing data, and metadata as used across Refinitiv Data Platform APIs.\",\n  \"type\": \"object\",\n  \"required\": [\"ric\"],\n  \"properties\": {\n    \"ric\": {\n      \"type\": \"string\",\n      \"description\": \"Reuters Instrument Code (RIC) uniquely identifying the instrument on the Refinitiv platform.\",\n      \"pattern\": \"^[A-Z0-9.=/]+$\"\n    },\n    \"isin\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"International Securities Identification Number (ISIN) for the instrument.\",\n      \"pattern\": \"^[A-Z]{2}[A-Z0-9]{9}[0-9]$\",\n      \"minLength\": 12,\n      \"maxLength\": 12\n    },\n    \"cusip\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\"\
  : \"Committee on Uniform Securities Identification Procedures (CUSIP) number.\",\n      \"pattern\": \"^[A-Z0-9]{9}$\",\n      \"minLength\": 9,\n      \"maxLength\": 9\n    },\n    \"sedol\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Stock Exchange Daily Official List (SEDOL) code.\",\n      \"pattern\": \"^[A-Z0-9]{7}$\",\n      \"minLength\": 7,\n      \"maxLength\": 7\n    },\n    \"ticker\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Exchange ticker symbol for the instrument.\"\n    },\n    \"permId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Refinitiv Permanent Identifier (PermID) for the instrument.\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"lei\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Legal Entity Identifier (LEI) for the issuing organization.\",\n      \"pattern\": \"^[A-Z0-9]{20}$\",\n      \"minLength\": 20,\n      \"maxLength\": 20\n    },\n    \"displayName\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Human-readable display name of the instrument.\"\n    },\n    \"currency\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ISO 4217 currency code for the instrument's trading currency.\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"minLength\": 3,\n      \"maxLength\": 3\n    },\n    \"exchangeCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Market Identifier Code (MIC) for the exchange where the instrument is traded.\",\n      \"pattern\": \"^[A-Z]{4}$\"\n    },\n    \"exchangeName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Human-readable name of the exchange.\"\n    },\n    \"assetClass\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The asset class category of the instrument.\",\n      \"enum\": [\"Equity\", \"FixedIncome\", \"Commodity\", \"ForeignExchange\", \"Derivative\", \"Fund\", \"Index\", null]\n    },\n\
  \    \"country\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ISO 3166-1 alpha-2 country code of the primary listing.\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"status\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Current trading status of the instrument.\",\n      \"enum\": [\"Active\", \"Inactive\", \"Delisted\", null]\n    }\n  },\n  \"$defs\": {\n    \"PricingData\": {\n      \"type\": \"object\",\n      \"description\": \"Real-time or delayed pricing snapshot for an instrument.\",\n      \"properties\": {\n        \"bid\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Current best bid price.\"\n        },\n        \"ask\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Current best ask price.\"\n        },\n        \"last\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Last traded price.\"\n        },\n        \"open\": {\n     \
  \     \"type\": [\"number\", \"null\"],\n          \"description\": \"Opening price for the current trading session.\"\n        },\n        \"high\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Highest price in the current trading session.\"\n        },\n        \"low\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Lowest price in the current trading session.\"\n        },\n        \"close\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Previous session closing price.\"\n        },\n        \"volume\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Trading volume for the current session.\",\n          \"minimum\": 0\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp of the pricing data.\"\n        }\n      }\n    },\n    \"HistoricalBar\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"A single OHLCV bar from historical pricing data.\",\n      \"properties\": {\n        \"date\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"The date of the bar for interday data.\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp for intraday bars.\"\n        },\n        \"open\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Opening price.\"\n        },\n        \"high\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Highest price.\"\n        },\n        \"low\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Lowest price.\"\n        },\n        \"close\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Closing price.\"\n        },\n        \"volume\": {\n          \"type\": [\"integer\"\
  , \"null\"],\n          \"description\": \"Trading volume.\",\n          \"minimum\": 0\n        },\n        \"count\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Number of trades.\",\n          \"minimum\": 0\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/refinitiv/refs/heads/main/json-schema/refinitiv-instrument-schema.json
tags: []
title: Refinitiv Financial Instrument
---
