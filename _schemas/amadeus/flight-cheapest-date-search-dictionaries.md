---
description: ''
layout: schema
name: Dictionaries
properties_list:
- description: ''
  name: currencies
  type: object
- description: ''
  name: locations
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-cheapest-date-search-dictionaries-schema.json
slug: flight-cheapest-date-search-dictionaries
source_filename: flight-cheapest-date-search-dictionaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Dictionaries\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currencies\": {\n      \"$ref\": \"#/definitions/CurrencyDictionary\"\n    },\n    \"locations\": {\n      \"$ref\": \"#/definitions/LocationDictionary\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-cheapest-date-search-dictionaries-schema.json
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
title: Dictionaries
---
