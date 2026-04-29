---
description: the deposit/prepay policy information applicable to the offer. It includes accepted payments, deadline and the amount due
layout: schema
name: HotelProduct_DepositPolicy
properties_list:
- description: Deposit-Prepay amount
  name: amount
  type: string
- description: 'The date and time of the deadline in ISO 8601[https://www.w3.org/TR/NOTE-datetime]. Example: 2010-08-14T13:00:00 Please note that this value is expressed in the hotels local time zone'
  name: deadline
  type: string
- description: ''
  name: description
  type: object
- description: ''
  name: acceptedPayments
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-depositpolicy-schema.json
slug: hotel-search-hotelproduct-depositpolicy
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_DepositPolicy\",\n  \"description\": \"the deposit/prepay policy information applicable to the offer. It includes accepted payments, deadline and the amount due\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"Deposit-Prepay amount\"\n    },\n    \"deadline\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time of the deadline in ISO 8601[https://www.w3.org/TR/NOTE-datetime]. \\n Example: 2010-08-14T13:00:00\\n Please note that this value is expressed in the hotels local time zone\"\n    },\n    \"description\": {\n      \"$ref\": \"#/definitions/QualifiedFreeText\"\n    },\n    \"acceptedPayments\": {\n      \"$ref\": \"#/definitions/HotelProduct_PaymentPolicy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-depositpolicy-schema.json
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
title: HotelProduct_DepositPolicy
---
