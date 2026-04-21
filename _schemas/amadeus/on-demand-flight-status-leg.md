---
description: ''
layout: schema
name: Leg
properties_list:
- description: 3-letter IATA code of the departure airport. e.g. LHR
  name: boardPointIataCode
  type: string
- description: 3-letter IATA code of the arrival airport. e.g. BKK
  name: offPointIataCode
  type: string
- description: ''
  name: aircraftEquipment
  type: object
- description: duration of the leg following standard [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601#Durations)
  name: scheduledLegDuration
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/on-demand-flight-status-leg-schema.json
slug: on-demand-flight-status-leg
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
title: Leg
---
