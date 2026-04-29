---
description: Represents a commercial real estate portfolio in the ARGUS Enterprise platform, used to organize and manage groups of properties under a unified investment strategy.
layout: schema
name: Argus Enterprise Portfolio
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
- description: Investment strategy classification
  name: strategy
  type: string
- description: Number of properties in the portfolio
  name: totalProperties
  type: integer
- description: Aggregate market value of all properties
  name: totalMarketValue
  type: number
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Record creation timestamp
  name: createdAt
  type: string
- description: Record last update timestamp
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-portfolio-schema.json
slug: argus-enterprise-portfolio
source_filename: argus-enterprise-portfolio-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.argusenterprise.com/schemas/argus-enterprise/portfolio.json\",\n  \"title\": \"Argus Enterprise Portfolio\",\n  \"description\": \"Represents a commercial real estate portfolio in the ARGUS Enterprise platform, used to organize and manage groups of properties under a unified investment strategy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique portfolio identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio description\"\n    },\n    \"strategy\": {\n      \"type\": \"string\",\n      \"enum\": [\"Core\", \"CorePlus\", \"ValueAdd\", \"Opportunistic\"],\n      \"description\": \"Investment strategy classification\"\n    },\n    \"\
  totalProperties\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of properties in the portfolio\"\n    },\n    \"totalMarketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Aggregate market value of all properties\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (ISO 4217)\",\n      \"default\": \"USD\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last update timestamp\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-portfolio-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Argus Enterprise Portfolio
---
