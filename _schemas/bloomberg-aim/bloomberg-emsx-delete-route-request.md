---
description: ''
layout: schema
name: DeleteRouteRequest
properties_list:
- description: Order sequence number
  name: EMSX_SEQUENCE
  type: integer
- description: Route ID to cancel
  name: EMSX_ROUTE_ID
  type: integer
provider_name: Bloomberg AIM
provider_slug: bloomberg-aim
schema_file: json-schema/bloomberg-emsx-delete-route-request-schema.json
slug: bloomberg-emsx-delete-route-request
source_filename: bloomberg-emsx-delete-route-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteRouteRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMSX_SEQUENCE\": {\n      \"type\": \"integer\",\n      \"description\": \"Order sequence number\"\n    },\n    \"EMSX_ROUTE_ID\": {\n      \"type\": \"integer\",\n      \"description\": \"Route ID to cancel\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-aim/refs/heads/main/json-schema/bloomberg-emsx-delete-route-request-schema.json
tags:
- Financial Data
- Market Data
- Order Management
- Portfolio Management
- Trading
title: DeleteRouteRequest
---
