---
description: ''
layout: schema
name: ModifyOrderRequest
properties_list:
- description: Order sequence number to modify
  name: EMSX_SEQUENCE
  type: integer
- description: New order quantity
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
  name: EMSX_NOTES
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-modify-order-request-schema.json
slug: bloomberg-emsx-modify-order-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ModifyOrderRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\",\n      \"description\": \"Order sequence number to modify\"\n    },\n    \"EMSX_AMOUNT\": {\n      \"type\": \"integer\",\n      \"description\": \"New order quantity\"\n    },\n    \"EMSX_ORDER_TYPE\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_LIMIT_PRICE\": {\n      \"type\": \"number\"\n    },\n    \"EMSX_STOP_PRICE\": {\n      \"type\": \"number\"\n    },\n    \"EMSX_TIF\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_NOTES\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-modify-order-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: ModifyOrderRequest
---
