---
description: ''
layout: schema
name: RouteOrderResponse
properties_list:
- description: ''
  name: EMSX_SEQUENCE
  type: integer
- description: Unique route identifier
  name: EMSX_ROUTE_ID
  type: integer
- description: ''
  name: MESSAGE
  type: string
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-route-order-response-schema.json
slug: bloomberg-emsx-route-order-response
source_filename: bloomberg-emsx-route-order-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RouteOrderResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\"\n    },\n    \"EMSX_ROUTE_ID\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique route identifier\"\n    },\n    \"MESSAGE\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-route-order-response-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: RouteOrderResponse
---
