---
description: traveler discount
layout: schema
name: Discount
properties_list:
- description: ''
  name: subType
  type: object
- description: city of residence
  name: cityName
  type: string
- description: ''
  name: travelerType
  type: object
- description: resident card number
  name: cardNumber
  type: string
- description: resident certificate number
  name: certificateNumber
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-discount-schema.json
slug: flight-offers-price-discount
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-discount-schema.json\",\n  \"title\": \"Discount\",\n  \"description\": \"traveler discount\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subType\": {\n      \"$ref\": \"#/definitions/DiscountType\"\n    },\n    \"cityName\": {\n      \"type\": \"string\",\n      \"description\": \"city of residence\",\n      \"example\": \"MADRID\"\n    },\n    \"travelerType\": {\n      \"$ref\": \"#/definitions/DiscountTravelerType\"\n    },\n    \"cardNumber\": {\n      \"type\": \"string\",\n      \"description\": \"resident card number\",\n      \"example\": \"12568215Z\",\n      \"pattern\": \"[0-9A-Z][0-9]{0,12}[A-Z]\"\n    },\n    \"certificateNumber\": {\n      \"type\": \"string\",\n      \"description\": \"resident certificate number\",\n      \"example\": \"12568215Z\",\n  \
  \    \"pattern\": \"[0-9A-Z][0-9]{0,12}[A-Z]\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-discount-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Discount
---
