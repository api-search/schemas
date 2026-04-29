---
description: Confirmed cargo shipment booking
layout: schema
name: Shipment
properties_list:
- description: Air Waybill number
  name: awbNumber
  type: string
- description: Shipment status
  name: status
  type: string
- description: Origin airport IATA code
  name: origin
  type: string
- description: Destination airport IATA code
  name: destination
  type: string
- description: Ship date
  name: shipDate
  type: string
- description: Estimated delivery date
  name: estimatedDelivery
  type: string
- description: Total cargo charge in USD
  name: totalCharge
  type: number
- description: Charge currency
  name: currency
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-cargo-shipment-schema.json
slug: alaska-air-cargo-shipment
source_filename: alaska-air-cargo-shipment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-shipment-schema.json\",\n  \"title\": \"Shipment\",\n  \"description\": \"Confirmed cargo shipment booking\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awbNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Air Waybill number\",\n      \"example\": \"027-12345678\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Shipment status\",\n      \"enum\": [\n        \"Booked\",\n        \"In Transit\",\n        \"Delivered\",\n        \"Cancelled\"\n      ],\n      \"example\": \"Booked\"\n    },\n    \"origin\": {\n      \"type\": \"string\",\n      \"description\": \"Origin airport IATA code\",\n      \"example\": \"SEA\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Destination airport IATA code\"\
  ,\n      \"example\": \"HNL\"\n    },\n    \"shipDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Ship date\",\n      \"example\": \"2026-04-20\"\n    },\n    \"estimatedDelivery\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Estimated delivery date\",\n      \"example\": \"2026-04-21\"\n    },\n    \"totalCharge\": {\n      \"type\": \"number\",\n      \"description\": \"Total cargo charge in USD\",\n      \"example\": 385.5\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Charge currency\",\n      \"example\": \"USD\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-shipment-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: Shipment
---
