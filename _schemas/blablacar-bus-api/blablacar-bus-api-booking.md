---
description: A confirmed booking for one or more passengers on a BlaBlaCar Bus trip
layout: schema
name: Booking
properties_list:
- description: Unique booking identifier
  name: booking_id
  type: string
- description: Current booking status
  name: status
  type: string
- description: Partner's own reference identifier
  name: partner_reference
  type: string
- description: Total booking price
  name: total_price
  type: object
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
schema_file: json-schema/blablacar-bus-api-booking-schema.json
slug: blablacar-bus-api-booking
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
title: Booking
---
