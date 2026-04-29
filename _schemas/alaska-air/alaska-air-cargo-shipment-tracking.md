---
description: Shipment tracking details with event history
layout: schema
name: ShipmentTracking
properties_list:
- description: Air Waybill number
  name: awbNumber
  type: string
- description: Current status
  name: status
  type: string
- description: Origin airport IATA code
  name: origin
  type: string
- description: Destination airport IATA code
  name: destination
  type: string
- description: Current location IATA code
  name: currentLocation
  type: string
- description: Estimated delivery date
  name: estimatedDelivery
  type: string
- description: Tracking event history
  name: events
  type: array
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-cargo-shipment-tracking-schema.json
slug: alaska-air-cargo-shipment-tracking
source_filename: alaska-air-cargo-shipment-tracking-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-shipment-tracking-schema.json\",\n  \"title\": \"ShipmentTracking\",\n  \"description\": \"Shipment tracking details with event history\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awbNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Air Waybill number\",\n      \"example\": \"027-12345678\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status\",\n      \"example\": \"In Transit\"\n    },\n    \"origin\": {\n      \"type\": \"string\",\n      \"description\": \"Origin airport IATA code\",\n      \"example\": \"SEA\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Destination airport IATA code\",\n      \"example\": \"HNL\"\n    },\n    \"currentLocation\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Current location IATA code\",\n      \"example\": \"SEA\"\n    },\n    \"estimatedDelivery\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Estimated delivery date\",\n      \"example\": \"2026-04-21\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Tracking event history\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TrackingEvent\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-shipment-tracking-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: ShipmentTracking
---
