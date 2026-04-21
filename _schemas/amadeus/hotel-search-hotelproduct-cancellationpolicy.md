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
