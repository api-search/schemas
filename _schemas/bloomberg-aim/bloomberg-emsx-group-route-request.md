---
description: ''
layout: schema
name: GroupRouteRequest
properties_list:
- description: List of order sequence numbers to route as a group
  name: EMSX_SEQUENCE
  type: array
- description: Percentage of each order to route (0-100)
  name: EMSX_AMOUNT_PERCENT
  type: number
- description: ''
  name: EMSX_BROKER
  type: string
- description: ''
  name: EMSX_ORDER_TYPE
  type: string
- description: ''
  name: EMSX_LIMIT_PRICE
  type: number
- description: ''
  name: EMSX_TIF
  type: string
- description: ''
  name: EMSX_STRATEGY
  type: string
- description: ''
  name: EMSX_STRATEGY_PARAMS
  type: object
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-group-route-request-schema.json
slug: bloomberg-emsx-group-route-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupRouteRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"array\",\n      \"description\": \"List of order sequence numbers to route as a group\"\n    },\n    \"EMSX_AMOUNT_PERCENT\": {\n      \"type\": \"number\",\n      \"description\": \"Percentage of each order to route (0-100)\"\n    },\n    \"EMSX_BROKER\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_ORDER_TYPE\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_LIMIT_PRICE\": {\n      \"type\": \"number\"\n    },\n    \"EMSX_TIF\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_STRATEGY\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_STRATEGY_PARAMS\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-group-route-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: GroupRouteRequest
---
