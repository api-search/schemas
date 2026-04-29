---
description: ''
layout: schema
name: Flights
properties_list:
- description: Approximate score for ranking purposes calculated based on number of flights from / to the airport or city
  name: score
  type: number
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-most-traveled-destinations-flights-schema.json
slug: flight-most-traveled-destinations-flights
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Flights\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"score\": {\n      \"type\": \"number\",\n      \"format\": \"integer\",\n      \"description\": \"Approximate score for ranking purposes calculated based on number of flights from / to the airport or city\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-most-traveled-destinations-flights-schema.json
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
title: Flights
---
