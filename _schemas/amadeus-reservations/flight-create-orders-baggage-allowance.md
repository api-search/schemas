---
description: baggageAllowance
layout: schema
name: BaggageAllowance
properties_list:
- description: Total number of units
  name: quantity
  type: integer
- description: Weight of the baggage allowance
  name: weight
  type: integer
- description: Code to qualify unit as pounds or kilos
  name: weightUnit
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-baggage-allowance-schema.json
slug: flight-create-orders-baggage-allowance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-baggage-allowance-schema.json\",\n  \"title\": \"BaggageAllowance\",\n  \"description\": \"baggageAllowance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of units\",\n      \"example\": 1\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"Weight of the baggage allowance\",\n      \"example\": 20\n    },\n    \"weightUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Code to qualify unit as pounds or kilos\",\n      \"example\": \"KG\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-baggage-allowance-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: BaggageAllowance
---
