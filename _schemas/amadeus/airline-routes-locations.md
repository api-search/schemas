---
description: Description of a particular point or place in physical space
layout: schema
name: locations
properties_list:
- description: type of API result "location"
  name: type
  type: string
- description: Location sub-type (e.g. airport, port, rail-station, restaurant, atm...)
  name: subtype
  type: string
- description: Label associated to the location (e.g. Eiffel Tower, Madison Square)
  name: name
  type: string
- description: IATA location code
  name: iataCode
  type: string
- description: Geographic coordinates describing the position of any location on the surface of Earth
  name: geoCode
  type: object
- description: ''
  name: address
  type: object
- description: ''
  name: timeZone
  type: object
- description: ''
  name: metrics
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-routes-locations-schema.json
slug: airline-routes-locations
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
title: locations
---
