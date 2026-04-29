---
description: Co2Emission schema
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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-co2-emission-schema.json
slug: seat-map-display-co2-emission
source_filename: seat-map-display-co2-emission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-co2-emission-schema.json\",\n  \"title\": \"Co2Emission\",\n  \"description\": \"Co2Emission schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"weight\": {\n      \"description\": \"Weight of Co2 emitted for the concerned segment\",\n      \"type\": \"integer\",\n      \"example\": 90\n    },\n    \"weightUnit\": {\n      \"description\": \"Code to qualify unit as pounds or kilos\",\n      \"type\": \"string\",\n      \"example\": \"KG\"\n    },\n    \"cabin\": {\n      \"$ref\": \"#/definitions/TravelClass\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-co2-emission-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Co2Emission
---
