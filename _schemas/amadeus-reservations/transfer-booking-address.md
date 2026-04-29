---
description: address information
layout: schema
name: Address
properties_list:
- description: Address line with street, number, bulding, etc...
  name: line
  type: string
- description: Post office code number
  name: zip
  type: string
- description: Country code (two character standard IATA country code)
  name: countryCode
  type: string
- description: City, town or postal station
  name: cityName
  type: string
- description: State code (two character standard IATA state code)
  name: stateCode
  type: string
- description: latitude of the location
  name: latitude
  type: number
- description: longitude of the location
  name: longitude
  type: number
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-address-schema.json
slug: transfer-booking-address
source_filename: transfer-booking-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-address-schema.json\",\n  \"title\": \"Address\",\n  \"description\": \"address information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"line\": {\n      \"description\": \"Address line with street, number, bulding, etc...\",\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 70\n    },\n    \"zip\": {\n      \"description\": \"Post office code number\",\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 120\n    },\n    \"countryCode\": {\n      \"description\": \"Country code (two character standard IATA country code)\",\n      \"type\": \"string\",\n      \"pattern\": \"[a-zA-Z]{2}\"\n    },\n    \"cityName\": {\n      \"description\": \"City, town or postal station\",\n      \"type\": \"string\",\n      \"minLength\"\
  : 1,\n      \"maxLength\": 35\n    },\n    \"stateCode\": {\n      \"description\": \"State code (two character standard IATA state code)\",\n      \"type\": \"string\",\n      \"pattern\": \"[a-zA-Z0-9]{1-2}\"\n    },\n    \"latitude\": {\n      \"description\": \"latitude of the location\",\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"example\": 43.580418\n    },\n    \"longitude\": {\n      \"description\": \"longitude of the location\",\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"example\": 7.125102\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-address-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: Address
---
