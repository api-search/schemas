---
description: A segment of an itinerary used by a traveler between 2 locations at a given date and time using a particular transportation type FLIGHT or TRAIN
layout: schema
name: TravelSegment
properties_list:
- description: ''
  name: transportationType
  type: object
- description: The flight number or train number, e.g. AF380
  name: transportationNumber
  type: string
- description: ''
  name: departure
  type: object
- description: ''
  name: arrival
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-booking-travelsegment-schema.json
slug: transfer-booking-travelsegment
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
title: TravelSegment
---
