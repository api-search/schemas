---
description: ''
layout: schema
name: AvailabilityClass
properties_list:
- description: Number of seats bookable in a single request. Can not be higher than 9.
  name: numberOfBookableSeats
  type: number
- description: The code of the booking class, a.k.a. class of service or Reservations/Booking Designator (RBD)
  name: class
  type: string
- description: Status of the booking class when it is closed.
  name: closedStatus
  type: string
- description: ''
  name: tourAllotment
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-availabilityclass-schema.json
slug: flight-availibilities-search-availabilityclass
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
title: AvailabilityClass
---
