---
description: address of the departure location
layout: schema
name: AddressCommon
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
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/transfer-booking-address-common-schema.json
slug: transfer-booking-address-common
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-address-common-schema.json\",\n  \"title\": \"AddressCommon\",\n  \"description\": \"address of the departure location\",\n  \"properties\": {\n    \"line\": {\n      \"description\": \"Address line with street, number, bulding, etc...\",\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 70\n    },\n    \"zip\": {\n      \"description\": \"Post office code number\",\n      \"type\": \"string\",\n      \"minLength\": 1,\n      \"maxLength\": 120\n    },\n    \"countryCode\": {\n      \"description\": \"Country code (two character standard IATA country code)\",\n      \"type\": \"string\",\n      \"pattern\": \"[a-zA-Z]{2}\"\n    },\n    \"cityName\": {\n      \"description\": \"City, town or postal station\",\n      \"type\": \"string\",\n      \"minLength\"\
  : 1,\n      \"maxLength\": 35\n    },\n    \"stateCode\": {\n      \"description\": \"State code (two character standard IATA state code)\",\n      \"type\": \"string\",\n      \"pattern\": \"[a-zA-Z0-9]{1-2}\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/transfer-booking-address-common-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: AddressCommon
---
