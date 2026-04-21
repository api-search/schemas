---
description: ''
layout: schema
name: FlightFilters
properties_list:
- description: Allows to search a location outside the borders when a radius around a location is specified. Default is false.
  name: crossBorderAllowed
  type: boolean
- description: This flag enables/disables the possibility to have more overnight flights in Low Fare Search
  name: moreOvernightsAllowed
  type: boolean
- description: This option force to retrieve flight-offer with a departure and a return in the same airport
  name: returnToDepartureAirport
  type: boolean
- description: This flag enable/disable filtering of rail segment (TGV AIR, RAIL ...)
  name: railSegmentAllowed
  type: boolean
- description: This flag enable/disable filtering of bus segment
  name: busSegmentAllowed
  type: boolean
- description: Maximum flight time as a percentage relative to the shortest flight time available for the itinerary
  name: maxFlightTime
  type: number
- description: ''
  name: carrierRestrictions
  type: object
- description: Restriction towards cabins.
  name: cabinRestrictions
  type: array
- description: ''
  name: connectionRestriction
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-search-flightfilters-schema.json
slug: flight-offers-search-flightfilters
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
title: FlightFilters
---
