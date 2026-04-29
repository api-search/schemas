---
description: the guarantee policy information applicable to the offer. It includes accepted payments
layout: schema
name: HotelProduct_GuaranteePolicy
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: acceptedPayments
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-guaranteepolicy-schema.json
slug: hotel-search-hotelproduct-guaranteepolicy
source_filename: hotel-search-hotelproduct-guaranteepolicy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_GuaranteePolicy\",\n  \"description\": \"the guarantee policy information applicable to the offer. It includes accepted payments\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"$ref\": \"#/definitions/QualifiedFreeText\"\n    },\n    \"acceptedPayments\": {\n      \"$ref\": \"#/definitions/HotelProduct_PaymentPolicy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-guaranteepolicy-schema.json
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
title: HotelProduct_GuaranteePolicy
---
