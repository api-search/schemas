---
description: ''
layout: schema
name: Fill
properties_list:
- description: Parent order sequence number
  name: EMSX_SEQUENCE
  type: integer
- description: Route that was filled
  name: EMSX_ROUTE_ID
  type: integer
- description: Unique fill identifier
  name: EMSX_FILL_ID
  type: integer
- description: ''
  name: EMSX_TICKER
  type: string
- description: ''
  name: EMSX_SIDE
  type: string
- description: Quantity filled
  name: EMSX_FILL_AMOUNT
  type: integer
- description: Fill price
  name: EMSX_FILL_PRICE
  type: number
- description: Fill date (YYYYMMDD)
  name: EMSX_FILL_DATE
  type: string
- description: Fill time (HHMMSS)
  name: EMSX_FILL_TIME
  type: string
- description: ''
  name: EMSX_BROKER
  type: string
- description: Exchange where the fill occurred
  name: EMSX_EXCHANGE
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-fill-schema.json
slug: bloomberg-emsx-fill
source_filename: bloomberg-emsx-fill-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Fill\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent order sequence number\"\n    },\n    \"EMSX_ROUTE_ID\": {\n      \"type\": \"integer\",\n      \"description\": \"Route that was filled\"\n    },\n    \"EMSX_FILL_ID\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique fill identifier\"\n    },\n    \"EMSX_TICKER\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_SIDE\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_FILL_AMOUNT\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity filled\"\n    },\n    \"EMSX_FILL_PRICE\": {\n      \"type\": \"number\",\n      \"description\": \"Fill price\"\n    },\n    \"EMSX_FILL_DATE\": {\n      \"type\": \"string\",\n      \"description\": \"Fill date (YYYYMMDD)\"\n    },\n    \"EMSX_FILL_TIME\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Fill time (HHMMSS)\"\n    },\n    \"EMSX_BROKER\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_EXCHANGE\": {\n      \"type\": \"string\",\n      \"description\": \"Exchange where the fill occurred\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-fill-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Fill
---
