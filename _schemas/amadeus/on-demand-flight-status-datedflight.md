---
description: ''
layout: schema
name: DatedFlight
properties_list:
- description: the resource name
  name: type
  type: string
- description: the scheduled departure date
  name: scheduledDepartureDate
  type: string
- description: ''
  name: flightDesignator
  type: object
- description: the flight points of the flight. At least one departure, one arrival
  name: flightPoints
  type: array
- description: 'the list of segments of the datedFlight - definition of segment: the commercial unit corresponding to the passenger journey traveling between two points with the same flight (same flight designator)'
  name: segments
  type: array
- description: 'the list of legs of the datedFlight. - definition of leg: operation of the aircraft between a departure station and the next arrival station (between take off and landing)'
  name: legs
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/on-demand-flight-status-datedflight-schema.json
slug: on-demand-flight-status-datedflight
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
title: DatedFlight
---
