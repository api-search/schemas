---
description: Individual consumer purchase data record
layout: schema
name: ConsumerPurchaseRecord
properties_list:
- description: Consumer demographic segment
  name: segment
  type: string
- description: Product category name
  name: category
  type: string
- description: Category penetration percentage
  name: penetration_pct
  type: number
- description: Average purchase frequency
  name: buy_rate
  type: number
- description: Average spend per buyer
  name: avg_spend
  type: number
- description: Average shopping trips per buyer
  name: trips_per_buyer
  type: number
- description: Retail channel
  name: channel
  type: string
provider_name: Circana
provider_slug: circana
schema_file: json-schema/liquid-data-consumer-purchase-record-schema.json
slug: liquid-data-consumer-purchase-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-consumer-purchase-record-schema.json\",\n  \"title\": \"ConsumerPurchaseRecord\",\n  \"description\": \"Individual consumer purchase data record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"segment\": {\n      \"type\": \"string\",\n      \"description\": \"Consumer demographic segment\",\n      \"example\": \"18-34\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Product category name\",\n      \"example\": \"Beverages\"\n    },\n    \"penetration_pct\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Category penetration percentage\",\n      \"example\": 72.5\n    },\n    \"buy_rate\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Average purchase frequency\",\n      \"\
  example\": 3.2\n    },\n    \"avg_spend\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Average spend per buyer\",\n      \"example\": 15.80\n    },\n    \"trips_per_buyer\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Average shopping trips per buyer\",\n      \"example\": 4.1\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"Retail channel\",\n      \"example\": \"grocery\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/circana/refs/heads/main/json-schema/liquid-data-consumer-purchase-record-schema.json
tags:
- Analytics
- Consumer Data
- Market Research
- Retail
- CPG
- Point Of Sale
- Consumer Insights
- Business Intelligence
title: ConsumerPurchaseRecord
---
