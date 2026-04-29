---
description: AvailableSeatsCounter schema
layout: schema
name: AvailableSeatsCounter
properties_list:
- description: Traveler id
  name: travelerId
  type: string
- description: Number of Seats with status AVAILABLE
  name: value
  type: integer
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/seat-map-display-available-seats-counter-schema.json
slug: seat-map-display-available-seats-counter
source_filename: seat-map-display-available-seats-counter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-available-seats-counter-schema.json\",\n  \"title\": \"AvailableSeatsCounter\",\n  \"description\": \"AvailableSeatsCounter schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"travelerId\": {\n      \"description\": \"Traveler id\",\n      \"type\": \"string\",\n      \"pattern\": \"[a-zA-Z0-9-]{1,20}\"\n    },\n    \"value\": {\n      \"description\": \"Number of Seats with status AVAILABLE\",\n      \"type\": \"integer\",\n      \"example\": 5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/seat-map-display-available-seats-counter-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: AvailableSeatsCounter
---
