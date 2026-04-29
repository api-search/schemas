---
description: A security position within a portfolio
layout: schema
name: Position
properties_list:
- description: Security identifier
  name: securityId
  type: string
- description: Security name
  name: securityName
  type: string
- description: Number of shares or units held
  name: quantity
  type: number
- description: Current market value in portfolio base currency
  name: marketValue
  type: number
- description: Portfolio weight as decimal
  name: weight
  type: number
- description: Security trading currency
  name: currency
  type: string
- description: Asset class classification
  name: assetClass
  type: string
- description: GICS sector
  name: sector
  type: string
provider_name: Aladdin Studio
provider_slug: aladdin-studio
schema_file: json-schema/aladdin-studio-graph-position-schema.json
slug: aladdin-studio-graph-position
source_filename: aladdin-studio-graph-position-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-position-schema.json\",\n  \"title\": \"Position\",\n  \"description\": \"A security position within a portfolio\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securityId\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier\",\n      \"example\": \"US0378331005\"\n    },\n    \"securityName\": {\n      \"type\": \"string\",\n      \"description\": \"Security name\",\n      \"example\": \"Apple Inc\"\n    },\n    \"quantity\": {\n      \"type\": \"number\",\n      \"description\": \"Number of shares or units held\",\n      \"example\": 1000\n    },\n    \"marketValue\": {\n      \"type\": \"number\",\n      \"description\": \"Current market value in portfolio base currency\",\n      \"example\": 195000.0\n    },\n    \"weight\": {\n      \"type\":\
  \ \"number\",\n      \"description\": \"Portfolio weight as decimal\",\n      \"example\": 0.025\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Security trading currency\",\n      \"example\": \"USD\"\n    },\n    \"assetClass\": {\n      \"type\": \"string\",\n      \"description\": \"Asset class classification\",\n      \"example\": \"Equity\"\n    },\n    \"sector\": {\n      \"type\": \"string\",\n      \"description\": \"GICS sector\",\n      \"example\": \"Technology\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aladdin-studio/refs/heads/main/json-schema/aladdin-studio-graph-position-schema.json
tags:
- Financial
- Investment Management
- Portfolio Analytics
- Risk Management
- Asset Management
- BlackRock
- Data Cloud
title: Position
---
