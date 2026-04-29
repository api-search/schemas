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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-address-schema.json
slug: transfer-booking-address
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Address\",\n  \"description\": \"address information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"line\": {\n      \"type\": \"string\",\n      \"description\": \"Address line with street, number, bulding, etc...\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"Post office code number\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Country code (two character standard IATA country code)\"\n    },\n    \"cityName\": {\n      \"type\": \"string\",\n      \"description\": \"City, town or postal station\"\n    },\n    \"stateCode\": {\n      \"type\": \"string\",\n      \"description\": \"State code (two character standard IATA state code)\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"latitude of the location\"\n    },\n    \"longitude\": {\n     \
  \ \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"longitude of the location\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-booking-address-schema.json
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
title: Address
---
