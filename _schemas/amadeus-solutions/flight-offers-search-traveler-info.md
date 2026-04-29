---
description: TravelerInfo schema
layout: schema
name: TravelerInfo
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: travelerType
  type: object
- description: if type="HELD_INFANT", corresponds to the adult travelers's id who will share the seat
  name: associatedAdultId
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-traveler-info-schema.json
slug: flight-offers-search-traveler-info
source_filename: flight-offers-search-traveler-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-traveler-info-schema.json\",\n  \"title\": \"TravelerInfo\",\n  \"description\": \"TravelerInfo schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": 1\n    },\n    \"travelerType\": {\n      \"$ref\": \"#/definitions/TravelerType\"\n    },\n    \"associatedAdultId\": {\n      \"type\": \"string\",\n      \"description\": \"if type=\\\"HELD_INFANT\\\", corresponds to the adult travelers's id who will share the seat\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"travelerType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-traveler-info-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: TravelerInfo
---
