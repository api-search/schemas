---
description: ''
layout: schema
name: CreateOrderResponse
properties_list:
- description: Unique order sequence number assigned by EMSX
  name: EMSX_SEQUENCE
  type: integer
- description: Status message
  name: MESSAGE
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-create-order-response-schema.json
slug: bloomberg-emsx-create-order-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateOrderResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique order sequence number assigned by EMSX\"\n    },\n    \"MESSAGE\": {\n      \"type\": \"string\",\n      \"description\": \"Status message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-create-order-response-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: CreateOrderResponse
---
