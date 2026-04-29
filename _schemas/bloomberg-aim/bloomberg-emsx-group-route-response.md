---
description: ''
layout: schema
name: GroupRouteResponse
properties_list:
- description: Number of orders successfully routed
  name: numRouted
  type: integer
- description: ''
  name: MESSAGE
  type: string
- description: ''
  name: routeIds
  type: array
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-group-route-response-schema.json
slug: bloomberg-emsx-group-route-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupRouteResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"numRouted\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of orders successfully routed\"\n    },\n    \"MESSAGE\": {\n      \"type\": \"string\"\n    },\n    \"routeIds\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-group-route-response-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: GroupRouteResponse
---
