---
description: ''
layout: schema
name: Address
properties_list:
- description: name of the city of the location; equal to name if the location is a city
  name: cityName
  type: string
- description: IATA code of the city of the location; equal to IATAcode if the location is a city
  name: cityCode
  type: string
- description: name of the country of the location
  name: countryName
  type: string
- description: code of the country of the location in ISO standard
  name: countryCode
  type: string
- description: code of the state of the location if any
  name: stateCode
  type: string
- description: code of the region of the location in ISO standard
  name: regionCode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airport-nearest-relevant-address-schema.json
slug: airport-nearest-relevant-address
source_filename: airport-nearest-relevant-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Address\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cityName\": {\n      \"type\": \"string\",\n      \"description\": \"name of the city of the location; equal to name if the location is a city\"\n    },\n    \"cityCode\": {\n      \"type\": \"string\",\n      \"description\": \"IATA code of the city of the location; equal to IATAcode if the location is a city\"\n    },\n    \"countryName\": {\n      \"type\": \"string\",\n      \"description\": \"name of the country of the location\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"code of the country of the location in ISO standard\"\n    },\n    \"stateCode\": {\n      \"type\": \"string\",\n      \"description\": \"code of the state of the location if any\"\n    },\n    \"regionCode\": {\n      \"type\": \"string\",\n      \"description\": \"code of the region of the location in ISO standard\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airport-nearest-relevant-address-schema.json
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
