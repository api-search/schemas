---
description: ''
layout: schema
name: CreateOrderRequest
properties_list:
- description: Bloomberg security identifier
  name: EMSX_TICKER
  type: string
- description: Order quantity (number of shares/contracts)
  name: EMSX_AMOUNT
  type: integer
- description: Order type
  name: EMSX_ORDER_TYPE
  type: string
- description: Buy or sell
  name: EMSX_SIDE
  type: string
- description: Time in force
  name: EMSX_TIF
  type: string
- description: Limit price (required for LMT and STP LMT orders)
  name: EMSX_LIMIT_PRICE
  type: number
- description: Stop price (required for STP and STP LMT orders)
  name: EMSX_STOP_PRICE
  type: number
- description: Trading account identifier
  name: EMSX_ACCOUNT
  type: string
- description: Free-text notes attached to the order
  name: EMSX_NOTES
  type: string
- description: Handling instruction
  name: EMSX_HAND_INSTRUCTION
  type: string
- description: Name of the basket this order belongs to
  name: EMSX_BASKET_NAME
  type: string
- description: Contract for difference flag
  name: EMSX_CFD_FLAG
  type: string
- description: ''
  name: EMSX_CUSTOM_NOTE1
  type: string
- description: ''
  name: EMSX_CUSTOM_NOTE2
  type: string
- description: ''
  name: EMSX_CUSTOM_NOTE3
  type: string
- description: ''
  name: EMSX_CUSTOM_NOTE4
  type: string
- description: ''
  name: EMSX_CUSTOM_NOTE5
  type: string
- description: Good-till-date in YYYYMMDD format
  name: EMSX_GTD_DATE
  type: string
- description: Investor identifier for allocation
  name: EMSX_INVESTOR_ID
  type: string
- description: Locate broker for short sells
  name: EMSX_LOCATE_BROKER
  type: string
- description: Locate ID for short sells
  name: EMSX_LOCATE_ID
  type: string
- description: Portfolio name for the order
  name: EMSX_PORTFOLIO
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-create-order-request-schema.json
slug: bloomberg-emsx-create-order-request
source_filename: bloomberg-emsx-create-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateOrderRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_TICKER\": {\n      \"type\": \"string\",\n      \"description\": \"Bloomberg security identifier\"\n    },\n    \"EMSX_AMOUNT\": {\n      \"type\": \"integer\",\n      \"description\": \"Order quantity (number of shares/contracts)\"\n    },\n    \"EMSX_ORDER_TYPE\": {\n      \"type\": \"string\",\n      \"description\": \"Order type\"\n    },\n    \"EMSX_SIDE\": {\n      \"type\": \"string\",\n      \"description\": \"Buy or sell\"\n    },\n    \"EMSX_TIF\": {\n      \"type\": \"string\",\n      \"description\": \"Time in force\"\n    },\n    \"EMSX_LIMIT_PRICE\": {\n      \"type\": \"number\",\n      \"description\": \"Limit price (required for LMT and STP LMT orders)\"\n    },\n    \"EMSX_STOP_PRICE\": {\n      \"type\": \"number\",\n      \"description\": \"Stop price (required for STP and STP LMT orders)\"\n\
  \    },\n    \"EMSX_ACCOUNT\": {\n      \"type\": \"string\",\n      \"description\": \"Trading account identifier\"\n    },\n    \"EMSX_NOTES\": {\n      \"type\": \"string\",\n      \"description\": \"Free-text notes attached to the order\"\n    },\n    \"EMSX_HAND_INSTRUCTION\": {\n      \"type\": \"string\",\n      \"description\": \"Handling instruction\"\n    },\n    \"EMSX_BASKET_NAME\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the basket this order belongs to\"\n    },\n    \"EMSX_CFD_FLAG\": {\n      \"type\": \"string\",\n      \"description\": \"Contract for difference flag\"\n    },\n    \"EMSX_CUSTOM_NOTE1\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_CUSTOM_NOTE2\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_CUSTOM_NOTE3\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_CUSTOM_NOTE4\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_CUSTOM_NOTE5\": {\n      \"type\": \"string\"\n    },\n    \"EMSX_GTD_DATE\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Good-till-date in YYYYMMDD format\"\n    },\n    \"EMSX_INVESTOR_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Investor identifier for allocation\"\n    },\n    \"EMSX_LOCATE_BROKER\": {\n      \"type\": \"string\",\n      \"description\": \"Locate broker for short sells\"\n    },\n    \"EMSX_LOCATE_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Locate ID for short sells\"\n    },\n    \"EMSX_PORTFOLIO\": {\n      \"type\": \"string\",\n      \"description\": \"Portfolio name for the order\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-create-order-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: CreateOrderRequest
---
