---
description: ''
layout: schema
name: AssignTraderRequest
properties_list:
- description: Order sequence number
  name: EMSX_SEQUENCE
  type: integer
- description: UUID of the trader to assign
  name: EMSX_TRADER_UUID
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-assign-trader-request-schema.json
slug: bloomberg-emsx-assign-trader-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssignTraderRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\",\n      \"description\": \"Order sequence number\"\n    },\n    \"EMSX_TRADER_UUID\": {\n      \"type\": \"string\",\n      \"description\": \"UUID of the trader to assign\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-assign-trader-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: AssignTraderRequest
---
