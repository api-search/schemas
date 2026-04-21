---
description: defining a flight segment; including both operating and marketing details when applicable
layout: schema
name: FlightSegment
properties_list:
- description: ''
  name: departure
  type: object
- description: ''
  name: arrival
  type: object
- description: providing the airline / carrier code
  name: carrierCode
  type: string
- description: the flight number as assigned by the carrier
  name: number
  type: string
- description: the flight number suffix as assigned by the carrier
  name: suffix
  type: string
- description: ''
  name: aircraft
  type: object
- description: reservation booking designator (RBD) of the carrier
  name: class
  type: string
- description: booking cabin / class of service of the carrier
  name: cabin
  type: string
- description: ''
  name: operating
  type: object
- description: stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M
  name: duration
  type: string
- description: information regarding the different stops composing the flight segment. E.g. technical stop, change of gauge...
  name: stops
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-choice-prediction-flightsegment-schema.json
slug: flight-choice-prediction-flightsegment
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
title: FlightSegment
---
