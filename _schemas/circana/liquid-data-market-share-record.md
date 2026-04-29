---
description: Individual market share data record
layout: schema
name: MarketShareRecord
properties_list:
- description: Brand name
  name: brand
  type: string
- description: Dollar market share percentage
  name: dollar_share
  type: number
- description: Unit market share percentage
  name: unit_share
  type: number
- description: Share change vs prior period in percentage points
  name: share_change
  type: number
- description: Time period identifier
  name: period
  type: string
provider_name: Circana
provider_slug: circana
schema_file: json-schema/liquid-data-market-share-record-schema.json
slug: liquid-data-market-share-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-market-share-record-schema.json\",\n  \"title\": \"MarketShareRecord\",\n  \"description\": \"Individual market share data record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Brand name\",\n      \"example\": \"Example Brand A\"\n    },\n    \"dollar_share\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Dollar market share percentage\",\n      \"example\": 24.5\n    },\n    \"unit_share\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Unit market share percentage\",\n      \"example\": 22.1\n    },\n    \"share_change\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Share change vs prior period in\
  \ percentage points\",\n      \"example\": 1.2\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"Time period identifier\",\n      \"example\": \"2026-Q1\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-market-share-record-schema.json
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
title: MarketShareRecord
---
