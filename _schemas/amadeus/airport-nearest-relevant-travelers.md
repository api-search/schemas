---
description: ''
layout: schema
name: Travelers
properties_list:
- description: Approximate score for ranking purposes calculated based on number of travelers in the location.
  name: score
  type: number
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airport-nearest-relevant-travelers-schema.json
slug: airport-nearest-relevant-travelers
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Travelers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"score\": {\n      \"type\": \"number\",\n      \"format\": \"integer\",\n      \"description\": \"Approximate score for ranking purposes calculated based on number of travelers in the location.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airport-nearest-relevant-travelers-schema.json
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
title: Travelers
---
