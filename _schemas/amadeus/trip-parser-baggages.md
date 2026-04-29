---
description: ''
layout: schema
name: baggages
properties_list:
- description: Total number of units
  name: quantity
  type: integer
- description: ''
  name: weight
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-baggages-schema.json
slug: trip-parser-baggages
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"baggages\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of units\"\n    },\n    \"weight\": {\n      \"$ref\": \"#/definitions/weight\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-baggages-schema.json
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
title: baggages
---
