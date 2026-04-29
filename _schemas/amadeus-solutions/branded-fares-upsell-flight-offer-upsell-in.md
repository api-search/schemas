---
description: input parameter to upsell flight offers element
layout: schema
name: FlightOfferUpsellIn
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
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/branded-fares-upsell-flight-offer-upsell-in-schema.json
slug: branded-fares-upsell-flight-offer-upsell-in
source_filename: branded-fares-upsell-flight-offer-upsell-in-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-flight-offer-upsell-in-schema.json\",\n  \"title\": \"FlightOfferUpsellIn\",\n  \"description\": \"input parameter to upsell flight offers element\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"description\": \"the resource name\",\n      \"type\": \"string\",\n      \"example\": \"flight-offer-upsell\"\n    },\n    \"flightOffers\": {\n      \"description\": \"list of flight offer to price\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightOffer\"\n      }\n    },\n    \"payments\": {\n      \"description\": \"payment information for retrieve eventual credit card fees\",\n      \"type\": \"array\",\n      \"maxItems\": 6,\n      \"items\": {\n        \"$ref\": \"\
  #/definitions/Payment\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"flightOffers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/branded-fares-upsell-flight-offer-upsell-in-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: FlightOfferUpsellIn
---
