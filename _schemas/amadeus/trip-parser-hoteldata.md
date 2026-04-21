---
description: Hotel product
layout: schema
name: hotelData
properties_list:
- description: Confirmation number
  name: confirmationNumber
  type: string
- description: heck-in date of the stay (hotel local date). Format YYYY-MM-DD The lowest accepted value is today date (no dates in the past).
  name: checkInDate
  type: string
- description: check-out date of the stay (hotel local date). Format YYYY-MM-DD The lowest accepted value is checkInDate+1.
  name: checkOutDate
  type: string
- description: number of rooms (1-9)
  name: roomQuantity
  type: integer
- description: ''
  name: contact
  type: object
- description: ''
  name: address
  type: object
- description: amenities (list)
  name: amenities
  type: array
- description: Hotel Name
  name: name
  type: string
- description: ''
  name: description
  type: object
- description: ''
  name: policies
  type: object
- description: ''
  name: guests
  type: object
- description: ''
  name: room
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-hoteldata-schema.json
slug: trip-parser-hoteldata
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
title: hotelData
---
