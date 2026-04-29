---
description: address information
layout: schema
name: Address
properties_list:
- description: Category of the contact element
  name: category
  type: string
- description: Line 1 = Street address, Line 2 = Apartment, suite, unit, building, floor, etc
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
- description: State code - two character standard [ISO 3166-2 state code](https://en.wikipedia.org/wiki/ISO_3166-2)
  name: stateCode
  type: string
- description: Full state name
  name: stateName
  type: string
- description: E.g. BP 220
  name: postalBox
  type: string
- description: Field containing a full unformatted address. Only applicable when the fields lines, postalCode, countryCode, cityName are not filled.
  name: text
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-address-schema.json
slug: seatmap-display-address
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Address\",\n  \"description\": \"address information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category of the contact element\",\n      \"enum\": [\n        \"BUSINESS\",\n        \"PERSONAL\",\n        \"OTHER\"\n      ]\n    },\n    \"lines\": {\n      \"type\": \"array\",\n      \"description\": \"Line 1 = Street address, Line 2 = Apartment, suite, unit, building, floor, etc\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"Example: 74130\"\n    },\n    \"countryCode\": {\n      \"type\": \"string\",\n      \"description\": \"country code [ISO 3166-1 country code](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)\"\n    },\n    \"cityName\": {\n      \"type\": \"string\",\n      \"description\": \"Full city name. Example:\
  \ Dublin\"\n    },\n    \"stateCode\": {\n      \"type\": \"string\",\n      \"description\": \"State code - two character standard [ISO 3166-2 state code](https://en.wikipedia.org/wiki/ISO_3166-2)\"\n    },\n    \"stateName\": {\n      \"type\": \"string\",\n      \"description\": \"Full state name\"\n    },\n    \"postalBox\": {\n      \"type\": \"string\",\n      \"description\": \"E.g. BP 220\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Field containing a full unformatted address. Only applicable when the fields lines, postalCode, countryCode, cityName are not filled.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-address-schema.json
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
