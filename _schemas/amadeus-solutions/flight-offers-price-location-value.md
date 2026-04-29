---
description: LocationValue schema
layout: schema
name: LocationValue
properties_list:
- description: City code associated to the airport
  name: cityCode
  type: string
- description: Country code of the airport
  name: countryCode
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-location-value-schema.json
slug: flight-offers-price-location-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-location-value-schema.json\",\n  \"title\": \"LocationValue\",\n  \"description\": \"LocationValue schema\",\n  \"properties\": {\n    \"cityCode\": {\n      \"type\": \"string\",\n      \"description\": \"City code associated to the airport\",\n      \"example\": \"PAR\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country code of the airport\",\n      \"example\": \"FR\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-location-value-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: LocationValue
---
