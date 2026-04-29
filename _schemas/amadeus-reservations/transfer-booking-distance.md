---
description: Distance schema
layout: schema
name: Distance
properties_list:
- description: 'great-circle distance between two locations. This distance thus do not take into account traffic conditions; international boundaries; mountains; water; or other elements that might make the a nearby '
  name: value
  type: integer
- description: unit of the distance
  name: unit
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-distance-schema.json
slug: transfer-booking-distance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-distance-schema.json\",\n  \"title\": \"Distance\",\n  \"description\": \"Distance schema\",\n  \"properties\": {\n    \"value\": {\n      \"description\": \"great-circle distance between two locations. This distance thus do not take into account traffic conditions; international boundaries; mountains; water; or other elements that might make the a nearby location hard to reach.\",\n      \"type\": \"integer\",\n      \"example\": 152\n    },\n    \"unit\": {\n      \"description\": \"unit of the distance\",\n      \"type\": \"string\",\n      \"example\": \"KM\",\n      \"enum\": [\n        \"KM\",\n        \"MI\"\n      ]\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-distance-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Distance
---
