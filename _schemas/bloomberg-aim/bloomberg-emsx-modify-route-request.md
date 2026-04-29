---
description: ''
layout: schema
name: ModifyRouteRequest
properties_list:
- description: Order sequence number
  name: EMSX_SEQUENCE
  type: integer
- description: Route ID to modify
  name: EMSX_ROUTE_ID
  type: integer
- description: ''
  name: EMSX_AMOUNT
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
- description: ''
  name: EMSX_STRATEGY
  type: string
- description: ''
  name: EMSX_STRATEGY_PARAMS
  type: object
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-modify-route-request-schema.json
slug: bloomberg-emsx-modify-route-request
source_filename: bloomberg-emsx-modify-route-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModifyRouteRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\",\n      \"description\": \"Order sequence number\"\n    },\n    \"EMSX_ROUTE_ID\": {\n      \"type\": \"integer\",\n      \"description\": \"Route ID to modify\"\n    },\n    \"EMSX_AMOUNT\": {\n      \"type\": \"integer\"\n    },\n    \"EMSX_ORDER_TYPE\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_LIMIT_PRICE\": {\n      \"type\": \"number\"\n    },\n    \"EMSX_STOP_PRICE\": {\n      \"type\": \"number\"\n    },\n    \"EMSX_TIF\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_STRATEGY\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_STRATEGY_PARAMS\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-modify-route-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: ModifyRouteRequest
---
