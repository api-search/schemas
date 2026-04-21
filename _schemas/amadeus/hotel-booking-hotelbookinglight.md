---
description: Booking Details
layout: schema
name: HotelBookingLight
properties_list:
- description: Response Type
  name: type
  type: string
- description: Booking Id
  name: id
  type: string
- description: GDS Confirmation Number. If you call the Provider, this Reference may be asked
  name: providerConfirmationId
  type: string
- description: ''
  name: associatedRecords
  type: array
- description: Retrieve Booking Details
  name: self
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-booking-hotelbookinglight-schema.json
slug: hotel-booking-hotelbookinglight
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
title: HotelBookingLight
---
