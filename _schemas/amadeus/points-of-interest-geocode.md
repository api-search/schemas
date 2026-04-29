---
description: ''
layout: schema
name: GeoCode
properties_list:
- description: latitude of the location
  name: latitude
  type: number
- description: longitude of the location
  name: longitude
  type: number
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/points-of-interest-geocode-schema.json
slug: points-of-interest-geocode
source_filename: points-of-interest-geocode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GeoCode\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"latitude of the location\"\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"longitude of the location\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/points-of-interest-geocode-schema.json
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
title: GeoCode
---
