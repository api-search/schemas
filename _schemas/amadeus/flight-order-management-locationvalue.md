---
description: ''
layout: schema
name: LocationValue
properties_list:
- description: City code associated to the airport
  name: cityCode
  type: string
- description: Country code of the airport
  name: countryCode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-order-management-locationvalue-schema.json
slug: flight-order-management-locationvalue
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"LocationValue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cityCode\": {\n      \"type\": \"string\",\n      \"description\": \"City code associated to the airport\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country code of the airport\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-order-management-locationvalue-schema.json
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
