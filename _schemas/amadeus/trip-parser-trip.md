---
description: ''
layout: schema
name: trip
properties_list:
- description: the resource name
  name: type
  type: string
- description: Reference of the Trip
  name: reference
  type: string
- description: Date of the trip point optional time and time offset in ISO 8601 format, e.g. 2017-02-10T20:40:00+02:00
  name: creationDateTime
  type: string
- description: itinerary booking date
  name: bookingDate
  type: string
- description: Ticket No(Specially for Air and Train segment)
  name: bookingNumber
  type: string
- description: information of the booking provider
  name: provider
  type: string
- description: Trip label or name
  name: title
  type: string
- description: Trip description
  name: description
  type: string
- description: ''
  name: start
  type: object
- description: ''
  name: end
  type: object
- description: ''
  name: travelAgency
  type: object
- description: ''
  name: stakeholders
  type: array
- description: ''
  name: price
  type: object
- description: ''
  name: products
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-trip-schema.json
slug: trip-parser-trip
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
title: trip
---
