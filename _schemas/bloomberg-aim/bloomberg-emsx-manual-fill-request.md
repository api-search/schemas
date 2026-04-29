---
description: ''
layout: schema
name: ManualFillRequest
properties_list:
- description: Order sequence number
  name: EMSX_SEQUENCE
  type: integer
- description: Route ID
  name: EMSX_ROUTE_ID
  type: integer
- description: Fill quantity
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
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-manual-fill-request-schema.json
slug: bloomberg-emsx-manual-fill-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManualFillRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\",\n      \"description\": \"Order sequence number\"\n    },\n    \"EMSX_ROUTE_ID\": {\n      \"type\": \"integer\",\n      \"description\": \"Route ID\"\n    },\n    \"EMSX_FILL_AMOUNT\": {\n      \"type\": \"integer\",\n      \"description\": \"Fill quantity\"\n    },\n    \"EMSX_FILL_PRICE\": {\n      \"type\": \"number\",\n      \"description\": \"Fill price\"\n    },\n    \"EMSX_FILL_DATE\": {\n      \"type\": \"string\",\n      \"description\": \"Fill date (YYYYMMDD)\"\n    },\n    \"EMSX_FILL_TIME\": {\n      \"type\": \"string\",\n      \"description\": \"Fill time (HHMMSS)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-manual-fill-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: ManualFillRequest
---
