---
description: ''
layout: schema
name: Order
properties_list:
- description: Unique order sequence number
  name: EMSX_SEQUENCE
  type: integer
- description: Security identifier
  name: EMSX_TICKER
  type: string
- description: ''
  name: EMSX_SIDE
  type: string
- description: Total order quantity
  name: EMSX_AMOUNT
  type: integer
- description: Quantity filled so far
  name: EMSX_FILLED
  type: integer
- description: Quantity currently working (routed but not filled)
  name: EMSX_WORKING
  type: integer
- description: ''
  name: EMSX_ORDER_TYPE
  type: string
- description: ''
  name: EMSX_LIMIT_PRICE
  type: number
- description: ''
  name: EMSX_STOP_PRICE
  type: number
- description: ''
  name: EMSX_TIF
  type: string
- description: Current order status
  name: EMSX_STATUS
  type: string
- description: Average fill price
  name: EMSX_AVG_PRICE
  type: number
- description: ''
  name: EMSX_ACCOUNT
  type: string
- description: ''
  name: EMSX_TRADER
  type: string
- description: ''
  name: EMSX_NOTES
  type: string
- description: ''
  name: EMSX_BASKET_NAME
  type: string
- description: Order creation date (YYYYMMDD)
  name: EMSX_DATE
  type: string
- description: Last update timestamp
  name: EMSX_TIME_STAMP
  type: string
- description: ''
  name: EMSX_PORTFOLIO
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-order-schema.json
slug: bloomberg-emsx-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Order\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique order sequence number\"\n    },\n    \"EMSX_TICKER\": {\n      \"type\": \"string\",\n      \"description\": \"Security identifier\"\n    },\n    \"EMSX_SIDE\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_AMOUNT\": {\n      \"type\": \"integer\",\n      \"description\": \"Total order quantity\"\n    },\n    \"EMSX_FILLED\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity filled so far\"\n    },\n    \"EMSX_WORKING\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity currently working (routed but not filled)\"\n    },\n    \"EMSX_ORDER_TYPE\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_LIMIT_PRICE\": {\n      \"type\": \"number\"\n    },\n    \"EMSX_STOP_PRICE\": {\n      \"type\": \"number\"\n    },\n\
  \    \"EMSX_TIF\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_STATUS\": {\n      \"type\": \"string\",\n      \"description\": \"Current order status\"\n    },\n    \"EMSX_AVG_PRICE\": {\n      \"type\": \"number\",\n      \"description\": \"Average fill price\"\n    },\n    \"EMSX_ACCOUNT\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_TRADER\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_NOTES\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_BASKET_NAME\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_DATE\": {\n      \"type\": \"string\",\n      \"description\": \"Order creation date (YYYYMMDD)\"\n    },\n    \"EMSX_TIME_STAMP\": {\n      \"type\": \"string\",\n      \"description\": \"Last update timestamp\"\n    },\n    \"EMSX_PORTFOLIO\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-order-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Order
---
