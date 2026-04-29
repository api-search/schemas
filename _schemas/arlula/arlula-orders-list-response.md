---
description: Paginated list of orders.
layout: schema
name: OrdersListResponse
properties_list:
- description: ''
  name: orders
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-orders-list-response-schema.json
slug: arlula-orders-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/orders-list-response.json\",\n  \"title\": \"OrdersListResponse\",\n  \"description\": \"Paginated list of orders.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orders\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"https://arlula.com/json-schema/order-response.json\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-orders-list-response-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: OrdersListResponse
---
