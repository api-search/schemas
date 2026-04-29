---
description: description of the aircraft equipment
layout: schema
name: aircraft
properties_list:
- description: aircraft type (ex 320, 777, ...)
  name: aircraftType
  type: string
- description: aircraft description (ex BOEING 737 ALL SERIES PASSENGER)
  name: aircraftDescription
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-aircraft-schema.json
slug: trip-parser-aircraft
source_filename: trip-parser-aircraft-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"aircraft\",\n  \"description\": \"description of the aircraft equipment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aircraftType\": {\n      \"type\": \"string\",\n      \"description\": \"aircraft type (ex 320, 777, ...)\"\n    },\n    \"aircraftDescription\": {\n      \"type\": \"string\",\n      \"description\": \"aircraft description (ex BOEING 737 ALL SERIES PASSENGER)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-aircraft-schema.json
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
title: aircraft
---
