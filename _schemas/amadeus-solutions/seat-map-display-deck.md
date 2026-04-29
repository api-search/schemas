---
description: deck information
layout: schema
name: Deck
properties_list:
- description: A deck is a level on an aircraft. The deck location of the cabin (current possible values are upper or main) The main deck, where passengers are seated on a passenger flight. Upper deck is above the m
  name: deckType
  type: string
- description: ''
  name: deckConfiguration
  type: object
- description: ''
  name: facilities
  type: array
- description: ''
  name: seats
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-deck-schema.json
slug: seat-map-display-deck
source_filename: seat-map-display-deck-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-deck-schema.json\",\n  \"title\": \"Deck\",\n  \"description\": \"deck information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deckType\": {\n      \"description\": \"A deck is a level on an aircraft. The deck location of the cabin (current possible values are upper or main) The main deck, where passengers are seated on a passenger flight. Upper deck is above the main deck where more passengers are seated.\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"UPPER\",\n        \"MAIN\",\n        \"LOWER\"\n      ]\n    },\n    \"deckConfiguration\": {\n      \"$ref\": \"#/definitions/DeckConfiguration\"\n    },\n    \"facilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Facility\"\n      }\n    },\n    \"seats\": {\n \
  \     \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Seat\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-deck-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Deck
---
