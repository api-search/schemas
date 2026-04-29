---
description: ''
layout: schema
name: Distance
properties_list:
- description: 'great-circle distance between two locations. This distance thus do not take into account traffic conditions; international boundaries; mountains; water; or other elements that might make the a nearby '
  name: value
  type: integer
- description: unit of the distance
  name: unit
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airport-city-search-distance-schema.json
slug: airport-city-search-distance
source_filename: airport-city-search-distance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Distance\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"integer\",\n      \"description\": \"great-circle distance between two locations. This distance thus do not take into account traffic conditions; international boundaries; mountains; water; or other elements that might make the a nearby location hard to reach.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"unit of the distance\",\n      \"enum\": [\n        \"KM\",\n        \"MI\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airport-city-search-distance-schema.json
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
title: Distance
---
