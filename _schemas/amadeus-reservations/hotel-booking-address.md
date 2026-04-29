---
description: Address information
layout: schema
name: Address
properties_list:
- description: Line 1 = Street address, Line 2 = Apartment, suite, unit, building, floor, etc
  name: lines
  type: array
- description: 'Example: 74130'
  name: postalCode
  type: string
- description: ISO 3166-1 country code
  name: countryCode
  type: string
- description: 'Full city name. Example: Dublin'
  name: cityName
  type: string
- description: State code (two character standard IATA state code)
  name: stateCode
  type: string
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/hotel-booking-address-schema.json
slug: hotel-booking-address
source_filename: hotel-booking-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"Address information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lines\": {\n      \"type\": \"array\",\n      \"description\": \"Line 1 = Street address, Line 2 = Apartment, suite, unit, building, floor, etc\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Example: 74130\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 country code\",\n      \"pattern\": \"[a-zA-Z]{2}\"\n    },\n    \"cityName\": {\n      \"type\": \"string\",\n      \"description\": \"Full city name. Example: Dublin\",\n      \"pattern\": \"[a-zA-Z -]{1,35}\"\n    },\n    \"stateCode\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"State code (two character standard IATA state code)\",\n      \"pattern\": \"[a-zA-Z0-9]{1,2}\"\n    }\n  },\n  \"required\": [\n    \"postalCode\",\n    \"countryCode\",\n    \"cityName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/hotel-booking-address-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Address
---
