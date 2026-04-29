---
description: ''
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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-travelerinfo-schema.json
slug: flight-availibilities-search-travelerinfo
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TravelerInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"travelerType\": {\n      \"$ref\": \"#/definitions/TravelerType\"\n    },\n    \"associatedAdultId\": {\n      \"type\": \"string\",\n      \"description\": \"if type=\\\"HELD_INFANT\\\", corresponds to the adult travelers's id who will share the seat\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"travelerType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-availibilities-search-travelerinfo-schema.json
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
title: TravelerInfo
---
