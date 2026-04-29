---
description: remarks
layout: schema
name: Remarks
properties_list:
- description: list of general remarks
  name: general
  type: array
- description: list of airline remarks
  name: airline
  type: array
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-remarks-schema.json
slug: flight-create-orders-remarks
source_filename: flight-create-orders-remarks-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-remarks-schema.json\",\n  \"title\": \"Remarks\",\n  \"description\": \"remarks\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"general\": {\n      \"description\": \"list of general remarks\",\n      \"type\": \"array\",\n      \"minItems\": 0,\n      \"maxItems\": 200,\n      \"items\": {\n        \"$ref\": \"#/definitions/GeneralRemark\"\n      }\n    },\n    \"airline\": {\n      \"description\": \"list of airline remarks\",\n      \"type\": \"array\",\n      \"minItems\": 0,\n      \"maxItems\": 200,\n      \"items\": {\n        \"$ref\": \"#/definitions/AirlineRemark\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-remarks-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Remarks
---
