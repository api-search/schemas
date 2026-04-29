---
description: ''
layout: schema
name: Links
properties_list:
- description: ''
  name: href
  type: string
- description: ''
  name: methods
  type: array
- description: ''
  name: count
  type: integer
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airport-city-search-links-schema.json
slug: airport-city-search-links
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Links\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"methods\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"GET\",\n          \"PUT\",\n          \"DELETE\",\n          \"POST\",\n          \"PATCH\"\n        ]\n      }\n    },\n    \"count\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"href\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airport-city-search-links-schema.json
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
title: Links
---
