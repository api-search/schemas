---
description: Request for cargo rate estimate
layout: schema
name: RateRequest
properties_list:
- description: Origin airport IATA code
  name: origin
  type: string
- description: Destination airport IATA code
  name: destination
  type: string
- description: Desired ship date
  name: shipDate
  type: string
- description: Shipment weight
  name: weight
  type: number
- description: Weight unit
  name: weightUnit
  type: string
- description: Number of pieces
  name: pieces
  type: integer
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-cargo-rate-request-schema.json
slug: alaska-air-cargo-rate-request
source_filename: alaska-air-cargo-rate-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-rate-request-schema.json\",\n  \"title\": \"RateRequest\",\n  \"description\": \"Request for cargo rate estimate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"origin\": {\n      \"type\": \"string\",\n      \"description\": \"Origin airport IATA code\",\n      \"example\": \"SEA\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Destination airport IATA code\",\n      \"example\": \"HNL\"\n    },\n    \"shipDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Desired ship date\",\n      \"example\": \"2026-04-20\"\n    },\n    \"weight\": {\n      \"type\": \"number\",\n      \"description\": \"Shipment weight\",\n      \"example\": 45.5\n    },\n    \"weightUnit\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Weight unit\",\n      \"enum\": [\n        \"KG\",\n        \"LB\"\n      ],\n      \"example\": \"KG\"\n    },\n    \"pieces\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of pieces\",\n      \"example\": 3\n    }\n  },\n  \"required\": [\n    \"origin\",\n    \"destination\",\n    \"shipDate\",\n    \"weight\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-rate-request-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: RateRequest
---
