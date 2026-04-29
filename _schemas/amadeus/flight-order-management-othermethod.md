---
description: other payment method
layout: schema
name: OtherMethod
properties_list:
- description: ''
  name: method
  type: object
- description: Id of the concern flightOffers
  name: flightOfferIds
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-order-management-othermethod-schema.json
slug: flight-order-management-othermethod
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"OtherMethod\",\n  \"description\": \"other payment method\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"method\": {\n      \"$ref\": \"#/definitions/OtherPaymentMethod\"\n    },\n    \"flightOfferIds\": {\n      \"type\": \"array\",\n      \"description\": \"Id of the concern flightOffers\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-order-management-othermethod-schema.json
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
title: OtherMethod
---
