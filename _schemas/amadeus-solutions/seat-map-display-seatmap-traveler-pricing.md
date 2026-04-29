---
description: SeatmapTravelerPricing schema
layout: schema
name: SeatmapTravelerPricing
properties_list:
- description: Traveler id
  name: travelerId
  type: string
- description: Seat availability for this specific traveler. Allows better seat choice per traveler
  name: seatAvailabilityStatus
  type: string
- description: Price for a given seat
  name: price
  type: object
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-seatmap-traveler-pricing-schema.json
slug: seat-map-display-seatmap-traveler-pricing
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-seatmap-traveler-pricing-schema.json\",\n  \"title\": \"SeatmapTravelerPricing\",\n  \"description\": \"SeatmapTravelerPricing schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"travelerId\": {\n      \"description\": \"Traveler id\",\n      \"type\": \"string\",\n      \"pattern\": \"[a-zA-Z0-9-]{1,20}\"\n    },\n    \"seatAvailabilityStatus\": {\n      \"description\": \"Seat availability for this specific traveler. Allows better seat choice per traveler\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"AVAILABLE\",\n        \"BLOCKED\",\n        \"OCCUPIED\"\n      ]\n    },\n    \"price\": {\n      \"description\": \"Price for a given seat\",\n      \"$ref\": \"#/definitions/Price\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-seatmap-traveler-pricing-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: SeatmapTravelerPricing
---
