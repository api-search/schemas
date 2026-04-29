---
description: ''
layout: schema
name: Route
properties_list:
- description: Parent order sequence number
  name: EMSX_SEQUENCE
  type: integer
- description: Unique route identifier
  name: EMSX_ROUTE_ID
  type: integer
- description: Broker code
  name: EMSX_BROKER
  type: string
- description: Routed quantity
  name: EMSX_AMOUNT
  type: integer
- description: Filled quantity on this route
  name: EMSX_FILLED
  type: integer
- description: ''
  name: EMSX_STATUS
  type: string
- description: ''
  name: EMSX_ORDER_TYPE
  type: string
- description: ''
  name: EMSX_LIMIT_PRICE
  type: number
- description: Average fill price for this route
  name: EMSX_AVG_PRICE
  type: number
- description: ''
  name: EMSX_STRATEGY
  type: string
- description: ''
  name: EMSX_EXEC_INSTRUCTIONS
  type: string
- description: ''
  name: EMSX_LAST_FILL_DATE
  type: string
- description: ''
  name: EMSX_LAST_FILL_TIME
  type: string
- description: ''
  name: EMSX_ROUTE_CREATE_DATE
  type: string
- description: ''
  name: EMSX_ROUTE_CREATE_TIME
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-route-schema.json
slug: bloomberg-emsx-route
source_filename: bloomberg-emsx-route-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Route\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent order sequence number\"\n    },\n    \"EMSX_ROUTE_ID\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique route identifier\"\n    },\n    \"EMSX_BROKER\": {\n      \"type\": \"string\",\n      \"description\": \"Broker code\"\n    },\n    \"EMSX_AMOUNT\": {\n      \"type\": \"integer\",\n      \"description\": \"Routed quantity\"\n    },\n    \"EMSX_FILLED\": {\n      \"type\": \"integer\",\n      \"description\": \"Filled quantity on this route\"\n    },\n    \"EMSX_STATUS\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_ORDER_TYPE\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_LIMIT_PRICE\": {\n      \"type\": \"number\"\n    },\n    \"EMSX_AVG_PRICE\": {\n      \"type\": \"number\",\n      \"description\": \"Average fill price\
  \ for this route\"\n    },\n    \"EMSX_STRATEGY\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_EXEC_INSTRUCTIONS\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_LAST_FILL_DATE\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_LAST_FILL_TIME\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_ROUTE_CREATE_DATE\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_ROUTE_CREATE_TIME\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-route-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: Route
---
