---
description: Description of a particular point or place in physical space
layout: schema
name: arrival
properties_list:
- description: Location sub-type (e.g. airport, port, rail-station, restaurant, atm...)
  name: subtype
  type: string
- description: Label associated to the location (e.g. Eiffel Tower, Madison Square)
  name: name
  type: string
- description: IATA location code
  name: iataCode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-arrival-schema.json
slug: trip-parser-arrival
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
title: arrival
---
