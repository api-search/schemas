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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-deck-schema.json
slug: seatmap-display-deck
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Deck\",\n  \"description\": \"deck information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deckType\": {\n      \"type\": \"string\",\n      \"description\": \"A deck is a level on an aircraft. The deck location of the cabin (current possible values are upper or main) The main deck, where passengers are seated on a passenger flight. Upper deck is above the main deck where more passengers are seated.\",\n      \"enum\": [\n        \"UPPER\",\n        \"MAIN\",\n        \"LOWER\"\n      ]\n    },\n    \"deckConfiguration\": {\n      \"$ref\": \"#/definitions/DeckConfiguration\"\n    },\n    \"facilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Facility\"\n      }\n    },\n    \"seats\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Seat\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-deck-schema.json
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
title: Deck
---
