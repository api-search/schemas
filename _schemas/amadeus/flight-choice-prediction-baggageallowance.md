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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-choice-prediction-baggageallowance-schema.json
slug: flight-choice-prediction-baggageallowance
source_filename: flight-choice-prediction-baggageallowance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"BaggageAllowance\",\n  \"description\": \"baggageAllowance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of units\"\n    },\n    \"weight\": {\n      \"type\": \"integer\",\n      \"description\": \"Weight of the baggage allowance\"\n    },\n    \"weightUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Code to qualify unit as pounds or kilos\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-choice-prediction-baggageallowance-schema.json
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
title: BaggageAllowance
---
