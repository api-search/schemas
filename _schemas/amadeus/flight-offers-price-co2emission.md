---
description: ''
layout: schema
name: Co2Emission
properties_list:
- description: Weight of Co2 emitted for the concerned segment
  name: weight
  type: integer
- description: Code to qualify unit as pounds or kilos
  name: weightUnit
  type: string
- description: ''
  name: cabin
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-co2emission-schema.json
slug: flight-offers-price-co2emission
source_filename: flight-offers-price-co2emission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Co2Emission\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"Weight of Co2 emitted for the concerned segment\"\n    },\n    \"weightUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Code to qualify unit as pounds or kilos\"\n    },\n    \"cabin\": {\n      \"$ref\": \"#/definitions/TravelClass\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-co2emission-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: Co2Emission
---
