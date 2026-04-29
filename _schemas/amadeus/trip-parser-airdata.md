---
description: ''
layout: schema
name: airData
properties_list:
- description: ''
  name: confirmationNumber
  type: string
- description: ''
  name: baggages
  type: object
- description: ''
  name: meal
  type: object
- description: ''
  name: departureAirportLocation
  type: object
- description: ''
  name: arrivalAirportLocation
  type: object
- description: ''
  name: departure
  type: object
- description: ''
  name: arrival
  type: object
- description: ''
  name: marketing
  type: object
- description: ''
  name: operating
  type: object
- description: ''
  name: aircraft
  type: object
- description: ''
  name: seats
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-airdata-schema.json
slug: trip-parser-airdata
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"airData\",\n  \"description\": \"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"confirmationNumber\": {\n      \"type\": \"string\"\n    },\n    \"baggages\": {\n      \"$ref\": \"#/definitions/baggages\"\n    },\n    \"meal\": {\n      \"$ref\": \"#/definitions/meal\"\n    },\n    \"departureAirportLocation\": {\n      \"$ref\": \"#/definitions/departureAirportLocation\"\n    },\n    \"arrivalAirportLocation\": {\n      \"$ref\": \"#/definitions/arrivalAirportLocation\"\n    },\n    \"departure\": {\n      \"$ref\": \"#/definitions/departureAir\"\n    },\n    \"arrival\": {\n      \"$ref\": \"#/definitions/arrivalAir\"\n    },\n    \"marketing\": {\n      \"$ref\": \"#/definitions/marketing\"\n    },\n    \"operating\": {\n      \"$ref\": \"#/definitions/operating\"\n    },\n    \"aircraft\": {\n      \"$ref\": \"#/definitions/aircraft\"\n    },\n    \"seats\": {\n      \"type\": \"array\"\
  ,\n      \"items\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/definitions/seats\"\n          },\n          {\n            \"type\": \"object\",\n            \"properties\": {\n              \"associationRefs\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"$ref\": \"#/definitions/associationRefs\"\n                }\n              }\n            }\n          }\n        ]\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-airdata-schema.json
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
title: airData
---
