---
description: ''
layout: schema
name: CreditCardFee
properties_list:
- description: ''
  name: brand
  type: object
- description: ''
  name: amount
  type: string
- description: ''
  name: currency
  type: string
- description: Id of the flightOffer concerned by the credit card fee
  name: flightOfferId
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-creditcardfee-schema.json
slug: flight-offers-price-creditcardfee
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreditCardFee\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"$ref\": \"#/definitions/PaymentBrand\"\n    },\n    \"amount\": {\n      \"type\": \"string\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"flightOfferId\": {\n      \"type\": \"string\",\n      \"description\": \"Id of the flightOffer concerned by the credit card fee\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-creditcardfee-schema.json
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
title: CreditCardFee
---
