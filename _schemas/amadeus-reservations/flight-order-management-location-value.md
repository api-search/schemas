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
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-location-value-schema.json
slug: flight-order-management-location-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-location-value-schema.json\",\n  \"title\": \"LocationValue\",\n  \"description\": \"LocationValue schema\",\n  \"properties\": {\n    \"cityCode\": {\n      \"type\": \"string\",\n      \"description\": \"City code associated to the airport\",\n      \"example\": \"PAR\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country code of the airport\",\n      \"example\": \"FR\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-location-value-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: LocationValue
---
