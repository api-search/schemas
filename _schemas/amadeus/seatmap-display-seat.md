---
description: ''
layout: schema
name: Seat
properties_list:
- description: Cabin of the seat.
  name: cabin
  type: string
- description: Concatenation of the row id and the column id, for example 12B
  name: number
  type: string
- description: 'List of seat characteristics (the characteristic''s names can be retrieved in the seat characteristic dictionary) Possible values are part of: IATA code: Most of the codes are defined by IATA Standard/'
  name: characteristicsCodes
  type: array
- description: Traveler's information and price
  name: travelerPricing
  type: array
- description: ''
  name: coordinates
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-seat-schema.json
slug: seatmap-display-seat
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
title: Seat
---
