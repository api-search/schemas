---
description: Accepted Payment Methods and Card Types. Several Payment Methods and Card Types may be available.
layout: schema
name: HotelProduct_PaymentPolicy
properties_list:
- description: Accepted Payment Card Types for the `method` CREDIT_CARD
  name: creditCards
  type: array
- description: Accepted Payment Methods
  name: methods
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-paymentpolicy-schema.json
slug: hotel-search-hotelproduct-paymentpolicy
source_filename: hotel-search-hotelproduct-paymentpolicy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_PaymentPolicy\",\n  \"description\": \"Accepted Payment Methods and Card Types. Several Payment Methods and Card Types may be available.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creditCards\": {\n      \"type\": \"array\",\n      \"description\": \"Accepted Payment Card Types for the `method` CREDIT_CARD\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"methods\": {\n      \"type\": \"array\",\n      \"description\": \"Accepted Payment Methods\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Method\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-paymentpolicy-schema.json
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
title: HotelProduct_PaymentPolicy
---
