---
description: Schema representing a financial instrument in the Refinitiv Eikon ecosystem, including pricing, identifiers, and metadata.
layout: schema
name: Refinitiv Eikon Financial Instrument
properties_list:
- description: Primary instrument identifier.
  name: instrumentId
  type: string
- description: Reuters Instrument Code (RIC) — primary identifier in the Refinitiv ecosystem.
  name: ric
  type: string
- description: International Securities Identification Number.
  name: isin
  type: string
- description: Committee on Uniform Securities Identification Procedures number.
  name: cusip
  type: string
- description: Stock Exchange Daily Official List identifier.
  name: sedol
  type: string
- description: Permanent Identifier (PermID) — globally unique, persistent LSEG identifier.
  name: permId
  type: string
- description: Human-readable display name for the instrument.
  name: displayName
  type: string
- description: Asset class of the instrument.
  name: assetClass
  type: string
- description: Exchange code where the instrument is traded.
  name: exchange
  type: string
- description: ISO 4217 currency code.
  name: currency
  type: string
- description: Current pricing data.
  name: pricing
  type: object
provider_name: Refinitiv Eikon
provider_slug: refinitiv-eikon
schema_file: json-schema/refinitiv-eikon-instrument-schema.json
slug: refinitiv-eikon-instrument
source_filename: refinitiv-eikon-instrument-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/refinitiv-eikon/json-schema/refinitiv-eikon-instrument-schema.json\",\n  \"title\": \"Refinitiv Eikon Financial Instrument\",\n  \"description\": \"Schema representing a financial instrument in the Refinitiv Eikon ecosystem, including pricing, identifiers, and metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instrumentId\": {\n      \"type\": \"string\",\n      \"description\": \"Primary instrument identifier.\"\n    },\n    \"ric\": {\n      \"type\": \"string\",\n      \"description\": \"Reuters Instrument Code (RIC) — primary identifier in the Refinitiv ecosystem.\",\n      \"examples\": [\"AAPL.O\", \"IBM.N\", \"MSFT.OQ\"]\n    },\n    \"isin\": {\n      \"type\": \"string\",\n      \"description\": \"International Securities Identification Number.\",\n      \"pattern\": \"^[A-Z]{2}[A-Z0-9]{9}[0-9]$\"\n    },\n    \"cusip\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Committee on Uniform Securities Identification Procedures number.\",\n      \"pattern\": \"^[0-9A-Z]{9}$\"\n    },\n    \"sedol\": {\n      \"type\": \"string\",\n      \"description\": \"Stock Exchange Daily Official List identifier.\"\n    },\n    \"permId\": {\n      \"type\": \"string\",\n      \"description\": \"Permanent Identifier (PermID) — globally unique, persistent LSEG identifier.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the instrument.\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"description\": \"Asset class of the instrument.\",\n      \"enum\": [\"Equity\", \"Bond\", \"Fund\", \"Futures\", \"Options\", \"FX\", \"Commodity\", \"Index\"]\n    },\n    \"exchange\": {\n      \"type\": \"string\",\n      \"description\": \"Exchange code where the instrument is traded.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"\
  description\": \"ISO 4217 currency code.\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"pricing\": {\n      \"type\": \"object\",\n      \"description\": \"Current pricing data.\",\n      \"properties\": {\n        \"last\": {\n          \"type\": \"number\",\n          \"description\": \"Last trade price.\"\n        },\n        \"open\": {\n          \"type\": \"number\",\n          \"description\": \"Opening price.\"\n        },\n        \"high\": {\n          \"type\": \"number\",\n          \"description\": \"Day high price.\"\n        },\n        \"low\": {\n          \"type\": \"number\",\n          \"description\": \"Day low price.\"\n        },\n        \"bid\": {\n          \"type\": \"number\",\n          \"description\": \"Best bid price.\"\n        },\n        \"ask\": {\n          \"type\": \"number\",\n          \"description\": \"Best ask price.\"\n        },\n        \"volume\": {\n          \"type\": \"integer\",\n          \"description\": \"Trading volume.\"\n\
  \        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp of the pricing data.\"\n        }\n      }\n    }\n  },\n  \"required\": [\"ric\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/refinitiv-eikon/refs/heads/main/json-schema/refinitiv-eikon-instrument-schema.json
tags:
- Analytics
- Financial Data
- Financial News
- Market Data
- Real-Time Data
- Trading
title: Refinitiv Eikon Financial Instrument
---
