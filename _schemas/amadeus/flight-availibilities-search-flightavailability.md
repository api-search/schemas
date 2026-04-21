---
description: ''
layout: schema
name: FlightAvailability
properties_list:
- description: the resource name
  name: type
  type: string
- description: Id of the flight availability
  name: id
  type: string
- description: Id of the originDestination in query
  name: originDestinationId
  type: string
- description: ''
  name: source
  type: object
- description: If true, inform that a ticketing will be required at booking step.
  name: instantTicketingRequired
  type: boolean
- description: If true, a payment card is mandatory to book this flight offer
  name: paymentCardRequired
  type: boolean
- description: duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M for a duration of 2h10m
  name: duration
  type: string
- description: ''
  name: segments
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-flightavailability-schema.json
slug: flight-availibilities-search-flightavailability
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
title: FlightAvailability
---
