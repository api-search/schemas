---
description: ''
layout: schema
name: Segment
properties_list:
- description: 3-letter IATA code of the departure airport. e.g. CDG
  name: boardPointIataCode
  type: string
- description: 3-letter IATA code of the arrival airport. e.g. AMS
  name: offPointIataCode
  type: string
- description: duration of the segment following standard [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601#Durations)
  name: scheduledSegmentDuration
  type: string
- description: ''
  name: partnership
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/on-demand-flight-status-segment-schema.json
slug: on-demand-flight-status-segment
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
title: Segment
---
