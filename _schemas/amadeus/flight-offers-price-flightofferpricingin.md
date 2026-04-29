---
description: input parameter to price flight offers element
layout: schema
name: FlightOfferPricingIn
properties_list:
- description: the resource name
  name: type
  type: string
- description: list of flight offer to price
  name: flightOffers
  type: array
- description: payment information for retrieve eventual credit card fees
  name: payments
  type: array
- description: list of travelers
  name: travelers
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-flightofferpricingin-schema.json
slug: flight-offers-price-flightofferpricingin
source_filename: flight-offers-price-flightofferpricingin-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightOfferPricingIn\",\n  \"description\": \"input parameter to price flight offers element\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\"\n    },\n    \"flightOffers\": {\n      \"type\": \"array\",\n      \"description\": \"list of flight offer to price\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightOffer\"\n      }\n    },\n    \"payments\": {\n      \"type\": \"array\",\n      \"description\": \"payment information for retrieve eventual credit card fees\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"brand\": {\n            \"$ref\": \"#/definitions/PaymentBrand\"\n          },\n          \"binNumber\": {\n            \"type\": \"integer\",\n            \"description\": \"The first 6 digits of the credit card\"\n          },\n          \"\
  flightOfferIds\": {\n            \"type\": \"array\",\n            \"description\": \"Id of the flightOffers to pay\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"travelers\": {\n      \"type\": \"array\",\n      \"description\": \"list of travelers\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Traveler\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"flightOffers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-flightofferpricingin-schema.json
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
title: FlightOfferPricingIn
---
