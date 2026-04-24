---
description: Electronic ticket for a passenger on a BlaBlaCar Bus trip
layout: schema
name: Ticket
properties_list:
- description: Unique ticket identifier
  name: ticket_id
  type: string
- description: Associated booking identifier
  name: booking_id
  type: string
- description: Full name of the ticket holder
  name: passenger_name
  type: string
- description: Departure date and time
  name: departure_datetime
  type: string
- description: Departure station name
  name: from_station
  type: string
- description: Arrival station name
  name: to_station
  type: string
- description: Assigned seat number
  name: seat_number
  type: string
- description: Current ticket status
  name: status
  type: string
- description: Base64-encoded QR code image
  name: qr_code
  type: string
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
schema_file: json-schema/blablacar-bus-api-ticket-schema.json
slug: blablacar-bus-api-ticket
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
title: Ticket
---
