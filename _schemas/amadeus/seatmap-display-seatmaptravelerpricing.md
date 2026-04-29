---
description: ''
layout: schema
name: SeatmapTravelerPricing
properties_list:
- description: Traveler id
  name: travelerId
  type: string
- description: Seat availability for this specific traveler. Allows better seat choice per traveler
  name: seatAvailabilityStatus
  type: string
- description: ''
  name: price
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-seatmaptravelerpricing-schema.json
slug: seatmap-display-seatmaptravelerpricing
source_filename: seatmap-display-seatmaptravelerpricing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"SeatmapTravelerPricing\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"travelerId\": {\n      \"type\": \"string\",\n      \"description\": \"Traveler id\"\n    },\n    \"seatAvailabilityStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Seat availability for this specific traveler. Allows better seat choice per traveler\",\n      \"enum\": [\n        \"AVAILABLE\",\n        \"BLOCKED\",\n        \"OCCUPIED\"\n      ]\n    },\n    \"price\": {\n      \"$ref\": \"#/definitions/Price\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-seatmaptravelerpricing-schema.json
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
title: SeatmapTravelerPricing
---
