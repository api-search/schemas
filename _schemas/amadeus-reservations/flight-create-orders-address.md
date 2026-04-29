---
description: address information
layout: schema
name: Address
properties_list:
- description: Line 1 = Street address, Line 2 = Apartment, suite, unit, building, floor, etc Each line is limited to 35 characters
  name: lines
  type: array
- description: 'Example: 74130'
  name: postalCode
  type: string
- description: country code [ISO 3166-1 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)
  name: countryCode
  type: string
- description: 'Full city name. Example: Dublin'
  name: cityName
  type: string
- description: Full state name
  name: stateName
  type: string
- description: E.g. BP 220
  name: postalBox
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-address-schema.json
slug: flight-create-orders-address
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"address information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lines\": {\n      \"type\": \"array\",\n      \"description\": \"Line 1 = Street address, Line 2 = Apartment, suite, unit, building, floor, etc \\nEach line is limited to 35 characters\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Example: 74130\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"country code [ISO 3166-1 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)\",\n      \"pattern\": \"[a-zA-Z]{2}\"\n    },\n    \"cityName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Full city name. Example: Dublin\",\n      \"pattern\": \"[a-zA-Z -]{1,35}\"\n    },\n    \"stateName\": {\n      \"type\": \"string\",\n      \"description\": \"Full state name\"\n    },\n    \"postalBox\": {\n      \"type\": \"string\",\n      \"description\": \"E.g. BP 220\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-address-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Address
---
