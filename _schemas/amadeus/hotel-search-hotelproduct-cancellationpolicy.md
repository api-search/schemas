---
description: ''
layout: schema
name: HotelProduct_CancellationPolicy
properties_list:
- description: ''
  name: type
  type: object
- description: Amount of the cancellation fee.
  name: amount
  type: string
- description: Number of nights due as fee in case of cancellation.
  name: numberOfNights
  type: integer
- description: Percentage of the total stay amount to be paid in case of cancellation. Value is between 0 and 100.
  name: percentage
  type: string
- description: 'Represents the deadline after which the penalty applies. DateTime is in ISO 8601 [https://www.w3.org/TR/NOTE-datetime]. Example: 2010-08-14T12:00:00+01:00 Example: 2010-08-14T12:00:00Z Example: 2010-0'
  name: deadline
  type: string
- description: ''
  name: description
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-search-hotelproduct-cancellationpolicy-schema.json
slug: hotel-search-hotelproduct-cancellationpolicy
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HotelProduct_CancellationPolicy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"$ref\": \"#/definitions/CancellationType\"\n    },\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"Amount of the cancellation fee.\"\n    },\n    \"numberOfNights\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Number of nights due as fee in case of cancellation.\"\n    },\n    \"percentage\": {\n      \"type\": \"string\",\n      \"description\": \"Percentage of the total stay amount to be paid in case of cancellation. Value is between 0 and 100.\"\n    },\n    \"deadline\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Represents the deadline after which the penalty applies. DateTime is in ISO 8601 [https://www.w3.org/TR/NOTE-datetime].\\nExample: 2010-08-14T12:00:00+01:00\\nExample:\
  \ 2010-08-14T12:00:00Z\\nExample: 2010-08-14T12:00:00-01:00\\nThe value is expressed in the hotel local time zone, with the added time zone difference. So you can compute the deadline in UTC(GMT) if desired.\"\n    },\n    \"description\": {\n      \"$ref\": \"#/definitions/QualifiedFreeText\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-search-hotelproduct-cancellationpolicy-schema.json
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
title: HotelProduct_CancellationPolicy
---
