---
description: A specific coach departure on a route with pricing and availability
layout: schema
name: Trip
properties_list:
- description: Unique trip identifier
  name: id
  type: string
- description: Associated route identifier
  name: route_id
  type: string
- description: Departure date and time
  name: departure_datetime
  type: string
- description: Arrival date and time
  name: arrival_datetime
  type: string
- description: Number of seats currently available
  name: available_seats
  type: integer
- description: Price with amount and currency
  name: price
  type: object
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
schema_file: json-schema/blablacar-bus-api-trip-schema.json
slug: blablacar-bus-api-trip
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
title: Trip
---
