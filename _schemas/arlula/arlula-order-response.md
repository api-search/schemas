---
description: Response after placing an imagery order.
layout: schema
name: OrderResponse
properties_list:
- description: Unique order identifier.
  name: orderId
  type: string
- description: Current order status.
  name: status
  type: string
- description: Time the order was created.
  name: createdAt
  type: string
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-order-response-schema.json
slug: arlula-order-response
source_filename: arlula-order-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/order-response.json\",\n  \"title\": \"OrderResponse\",\n  \"description\": \"Response after placing an imagery order.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique order identifier.\",\n      \"examples\": [\n        \"order-500123\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current order status.\",\n      \"examples\": [\n        \"processing\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"Time the order was created.\",\n      \"examples\": [\n        \"2026-04-19T09:00:00Z\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-order-response-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: OrderResponse
---
