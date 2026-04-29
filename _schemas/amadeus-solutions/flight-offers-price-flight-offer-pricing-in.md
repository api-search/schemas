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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-flight-offer-pricing-in-schema.json
slug: flight-offers-price-flight-offer-pricing-in
source_filename: flight-offers-price-flight-offer-pricing-in-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-flight-offer-pricing-in-schema.json\",\n  \"title\": \"FlightOfferPricingIn\",\n  \"description\": \"input parameter to price flight offers element\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"description\": \"the resource name\",\n      \"type\": \"string\",\n      \"example\": \"flight-offer-pricing\"\n    },\n    \"flightOffers\": {\n      \"description\": \"list of flight offer to price\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightOffer\"\n      }\n    },\n    \"payments\": {\n      \"description\": \"payment information for retrieve eventual credit card fees\",\n      \"type\": \"array\",\n      \"maxItems\": 6,\n      \"items\": {\n        \"title\": \"\
  Payment\",\n        \"type\": \"object\",\n        \"properties\": {\n          \"brand\": {\n            \"$ref\": \"#/definitions/PaymentBrand\"\n          },\n          \"binNumber\": {\n            \"description\": \"The first 6 digits of the credit card\",\n            \"type\": \"integer\",\n            \"example\": 123456,\n            \"pattern\": \"[0-9]{6}\"\n          },\n          \"flightOfferIds\": {\n            \"description\": \"Id of the flightOffers to pay\",\n            \"type\": \"array\",\n            \"minItems\": 1,\n            \"maxItems\": 6,\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"example\": \"1\"\n          }\n        }\n      }\n    },\n    \"travelers\": {\n      \"description\": \"list of travelers\",\n      \"type\": \"array\",\n      \"maxItems\": 18,\n      \"items\": {\n        \"$ref\": \"#/definitions/Traveler\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"flightOffers\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-flight-offer-pricing-in-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: FlightOfferPricingIn
---
