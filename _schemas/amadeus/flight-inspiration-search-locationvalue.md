---
description: ''
layout: schema
name: LocationValue
properties_list:
- description: 'location type: airport or city'
  name: subType
  type: string
- description: name of the location
  name: detailedName
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-inspiration-search-locationvalue-schema.json
slug: flight-inspiration-search-locationvalue
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"LocationValue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subType\": {\n      \"type\": \"string\",\n      \"description\": \"location type: airport or city\",\n      \"enum\": [\n        \"AIRPORT\",\n        \"CITY\"\n      ]\n    },\n    \"detailedName\": {\n      \"type\": \"string\",\n      \"description\": \"name of the location\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-inspiration-search-locationvalue-schema.json
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
title: LocationValue
---
