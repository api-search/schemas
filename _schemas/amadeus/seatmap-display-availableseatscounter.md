---
description: ''
layout: schema
name: AvailableSeatsCounter
properties_list:
- description: Traveler id
  name: travelerId
  type: string
- description: Number of Seats with status AVAILABLE
  name: value
  type: integer
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-availableseatscounter-schema.json
slug: seatmap-display-availableseatscounter
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AvailableSeatsCounter\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"travelerId\": {\n      \"type\": \"string\",\n      \"description\": \"Traveler id\"\n    },\n    \"value\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of Seats with status AVAILABLE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-availableseatscounter-schema.json
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
title: AvailableSeatsCounter
---
