---
description: The flight or train departure/arrival date&time, location information
layout: schema
name: TravelSegmentLocation
properties_list:
- description: The railway UIC code defined by the worldwide railway organization, e.g. 7400001
  name: uicCode
  type: string
- description: The airport code from IATA table codes, e.g. CDG
  name: iataCode
  type: string
- description: The date and time inspired from ISO 8601 (YYYY-MM-DDTHH:MM:SS) format
  name: localDateTime
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-search-travelsegmentlocation-schema.json
slug: transfer-search-travelsegmentlocation
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TravelSegmentLocation\",\n  \"description\": \"The flight or train departure/arrival date&time, location information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uicCode\": {\n      \"type\": \"string\",\n      \"description\": \"The railway UIC code defined by the worldwide railway organization, e.g. 7400001\"\n    },\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"The airport code from IATA table codes, e.g. CDG\"\n    },\n    \"localDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time inspired from ISO 8601 (YYYY-MM-DDTHH:MM:SS) format\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-search-travelsegmentlocation-schema.json
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
title: TravelSegmentLocation
---
