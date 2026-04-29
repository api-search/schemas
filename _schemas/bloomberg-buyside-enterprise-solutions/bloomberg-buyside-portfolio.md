---
description: A portfolio represents a collection of financial instrument holdings managed as a single entity for buy-side investment management, including trading portfolios, model portfolios, benchmarks, and composites.
layout: schema
name: Bloomberg Buyside Portfolio
properties_list:
- description: Unique portfolio identifier
  name: id
  type: string
- description: Portfolio name
  name: name
  type: string
- description: Portfolio description
  name: description
  type: string
- description: Portfolio type classification
  name: type
  type: string
- description: Current portfolio status
  name: status
  type: string
- description: Base currency for the portfolio (ISO 4217)
  name: currency
  type: string
- description: Identifier of the assigned benchmark for performance comparison
  name: benchmarkId
  type: string
- description: Portfolio manager identifier
  name: manager
  type: string
- description: Date the portfolio was established
  name: inceptionDate
  type: string
- description: Total current market value of the portfolio in base currency
  name: totalMarketValue
  type: number
- description: Number of distinct holdings in the portfolio
  name: holdingsCount
  type: integer
- description: Current portfolio holdings
  name: holdings
  type: array
- description: Timestamp when the portfolio was created
  name: createdAt
  type: string
- description: Timestamp of the most recent portfolio update
  name: updatedAt
  type: string
provider_name: Bloomberg Buyside Enterprise Solutions
provider_slug: bloomberg-buyside-enterprise-solutions
schema_file: json-schema/bloomberg-buyside-portfolio-schema.json
slug: bloomberg-buyside-portfolio
source_filename: bloomberg-buyside-portfolio-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.bloomberg.com/schemas/buyside/portfolio.json\",\n  \"title\": \"Bloomberg Buyside Portfolio\",\n  \"description\": \"A portfolio represents a collection of financial instrument holdings managed as a single entity for buy-side investment management, including trading portfolios, model portfolios, benchmarks, and composites.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"type\", \"currency\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique portfolio identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio name\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio description\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"TRADING\", \"MODEL\", \"BENCHMARK\"\
  , \"COMPOSITE\"],\n      \"description\": \"Portfolio type classification\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"ACTIVE\", \"INACTIVE\", \"CLOSED\"],\n      \"description\": \"Current portfolio status\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Base currency for the portfolio (ISO 4217)\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"benchmarkId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the assigned benchmark for performance comparison\"\n    },\n    \"manager\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio manager identifier\"\n    },\n    \"inceptionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the portfolio was established\"\n    },\n    \"totalMarketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Total current market value of the portfolio in base currency\"\n    },\n    \"\
  holdingsCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of distinct holdings in the portfolio\"\n    },\n    \"holdings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Holding\"\n      },\n      \"description\": \"Current portfolio holdings\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the portfolio was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the most recent portfolio update\"\n    }\n  },\n  \"$defs\": {\n    \"Holding\": {\n      \"type\": \"object\",\n      \"description\": \"A single position within a portfolio representing ownership of a financial instrument\",\n      \"required\": [\"security\", \"quantity\"],\n      \"properties\": {\n        \"security\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Bloomberg security identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Security display name\"\n        },\n        \"assetClass\": {\n          \"type\": \"string\",\n          \"description\": \"Asset class classification\"\n        },\n        \"quantity\": {\n          \"type\": \"number\",\n          \"description\": \"Number of shares or units held\"\n        },\n        \"marketValue\": {\n          \"type\": \"number\",\n          \"description\": \"Current market value in portfolio base currency\"\n        },\n        \"costBasis\": {\n          \"type\": \"number\",\n          \"description\": \"Total acquisition cost\"\n        },\n        \"weight\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"Portfolio weight as a percentage\"\n        },\n        \"unrealizedGainLoss\": {\n          \"type\": \"number\",\n          \"description\": \"Unrealized\
  \ profit or loss\"\n        },\n        \"sector\": {\n          \"type\": \"string\",\n          \"description\": \"GICS sector classification\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Country of risk (ISO 3166-1 alpha-2)\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"description\": \"Security trading currency (ISO 4217)\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-buyside-enterprise-solutions/refs/heads/main/json-schema/bloomberg-buyside-portfolio-schema.json
tags:
- Analytics
- Asset Management
- Buy-Side
- Enterprise Solutions
- Financial Services
- Market Data
- Portfolio Management
- Trading
title: Bloomberg Buyside Portfolio
---
