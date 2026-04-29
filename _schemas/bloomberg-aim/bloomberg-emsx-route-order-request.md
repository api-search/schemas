---
description: ''
layout: schema
name: RouteOrderRequest
properties_list:
- description: Order sequence number to route
  name: EMSX_SEQUENCE
  type: integer
- description: Quantity to route
  name: EMSX_AMOUNT
  type: integer
- description: Broker code
  name: EMSX_BROKER
  type: string
- description: ''
  name: EMSX_ORDER_TYPE
  type: string
- description: ''
  name: EMSX_TIF
  type: string
- description: ''
  name: EMSX_LIMIT_PRICE
  type: number
- description: ''
  name: EMSX_STOP_PRICE
  type: number
- description: Broker strategy name
  name: EMSX_STRATEGY
  type: string
- description: ''
  name: EMSX_STRATEGY_PARAMS
  type: object
- description: ''
  name: EMSX_EXEC_INSTRUCTIONS
  type: string
- description: ''
  name: EMSX_ACCOUNT
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-route-order-request-schema.json
slug: bloomberg-emsx-route-order-request
source_filename: bloomberg-emsx-route-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RouteOrderRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\",\n      \"description\": \"Order sequence number to route\"\n    },\n    \"EMSX_AMOUNT\": {\n      \"type\": \"integer\",\n      \"description\": \"Quantity to route\"\n    },\n    \"EMSX_BROKER\": {\n      \"type\": \"string\",\n      \"description\": \"Broker code\"\n    },\n    \"EMSX_ORDER_TYPE\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_TIF\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_LIMIT_PRICE\": {\n      \"type\": \"number\"\n    },\n    \"EMSX_STOP_PRICE\": {\n      \"type\": \"number\"\n    },\n    \"EMSX_STRATEGY\": {\n      \"type\": \"string\",\n      \"description\": \"Broker strategy name\"\n    },\n    \"EMSX_STRATEGY_PARAMS\": {\n      \"type\": \"object\"\n    },\n    \"EMSX_EXEC_INSTRUCTIONS\": {\n      \"type\": \"string\"\n    },\n \
  \   \"EMSX_ACCOUNT\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-route-order-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: RouteOrderRequest
---
