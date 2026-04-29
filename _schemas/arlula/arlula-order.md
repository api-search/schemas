---
description: A detailed order with campaigns and datasets.
layout: schema
name: Order
properties_list:
- description: Order identifier.
  name: orderId
  type: string
- description: Order status.
  name: status
  type: string
- description: Order creation timestamp.
  name: createdAt
  type: string
- description: ''
  name: campaigns
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-order-schema.json
slug: arlula-order
source_filename: arlula-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/order.json\",\n  \"title\": \"Order\",\n  \"description\": \"A detailed order with campaigns and datasets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Order identifier.\",\n      \"examples\": [\n        \"order-a1b2c3d4\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Order status.\",\n      \"examples\": [\n        \"completed\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"Order creation timestamp.\",\n      \"examples\": [\n        \"2026-04-15T09:00:00Z\"\n      ]\n    },\n    \"campaigns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"https://arlula.com/json-schema/campaign.json\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-order-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: Order
---
