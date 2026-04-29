---
description: Request body for creating a cargo shipment booking
layout: schema
name: ShipmentRequest
properties_list:
- description: Origin airport IATA code
  name: origin
  type: string
- description: Destination airport IATA code
  name: destination
  type: string
- description: Desired ship date (YYYY-MM-DD)
  name: shipDate
  type: string
- description: Commodity description
  name: commodity
  type: string
- description: Total shipment weight
  name: weight
  type: number
- description: Weight unit
  name: weightUnit
  type: string
- description: Number of pieces in shipment
  name: pieces
  type: integer
- description: ''
  name: dimensions
  type: object
- description: Special handling requirements
  name: specialHandling
  type: array
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-cargo-shipment-request-schema.json
slug: alaska-air-cargo-shipment-request
source_filename: alaska-air-cargo-shipment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-shipment-request-schema.json\",\n  \"title\": \"ShipmentRequest\",\n  \"description\": \"Request body for creating a cargo shipment booking\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"origin\": {\n      \"type\": \"string\",\n      \"description\": \"Origin airport IATA code\",\n      \"example\": \"SEA\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Destination airport IATA code\",\n      \"example\": \"HNL\"\n    },\n    \"shipDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Desired ship date (YYYY-MM-DD)\",\n      \"example\": \"2026-04-20\"\n    },\n    \"commodity\": {\n      \"type\": \"string\",\n      \"description\": \"Commodity description\",\n      \"example\": \"Electronics\"\n    },\n\
  \    \"weight\": {\n      \"type\": \"number\",\n      \"description\": \"Total shipment weight\",\n      \"example\": 45.5\n    },\n    \"weightUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Weight unit\",\n      \"enum\": [\n        \"KG\",\n        \"LB\"\n      ],\n      \"example\": \"KG\"\n    },\n    \"pieces\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of pieces in shipment\",\n      \"example\": 3\n    },\n    \"dimensions\": {\n      \"$ref\": \"#/components/schemas/Dimensions\"\n    },\n    \"specialHandling\": {\n      \"type\": \"array\",\n      \"description\": \"Special handling requirements\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"Fragile\"\n      ]\n    }\n  },\n  \"required\": [\n    \"origin\",\n    \"destination\",\n    \"shipDate\",\n    \"weight\",\n    \"pieces\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-shipment-request-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: ShipmentRequest
---
