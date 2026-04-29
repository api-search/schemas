---
description: Booking Rules
layout: schema
name: HotelProduct_PolicyDetails
properties_list:
- description: ''
  name: paymentType
  type: object
- description: ''
  name: guarantee
  type: object
- description: ''
  name: deposit
  type: object
- description: ''
  name: prepay
  type: object
- description: ''
  name: holdTime
  type: object
- description: ''
  name: cancellations
  type: array
- description: ''
  name: checkInOut
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-policydetails-schema.json
slug: hotel-search-hotelproduct-policydetails
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_PolicyDetails\",\n  \"description\": \"Booking Rules\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paymentType\": {\n      \"$ref\": \"#/definitions/PaymentType\"\n    },\n    \"guarantee\": {\n      \"$ref\": \"#/definitions/HotelProduct_GuaranteePolicy\"\n    },\n    \"deposit\": {\n      \"$ref\": \"#/definitions/HotelProduct_DepositPolicy\"\n    },\n    \"prepay\": {\n      \"$ref\": \"#/definitions/HotelProduct_DepositPolicy\"\n    },\n    \"holdTime\": {\n      \"$ref\": \"#/definitions/HotelProduct_HoldPolicy\"\n    },\n    \"cancellations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/HotelProduct_CancellationPolicy\"\n      }\n    },\n    \"checkInOut\": {\n      \"$ref\": \"#/definitions/HotelProduct_CheckInOutPolicy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-policydetails-schema.json
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
title: HotelProduct_PolicyDetails
---
