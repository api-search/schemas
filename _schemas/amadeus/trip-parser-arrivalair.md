---
description: Departure or arrival information
layout: schema
name: arrivalAir
properties_list:
- description: IATA Airport code
  name: iataCode
  type: string
- description: Terminal name / number
  name: terminal
  type: string
- description: Local schedule dateTime of the departure or arrival. Conversion of dateTime in local date time.
  name: localDateTime
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-arrivalair-schema.json
slug: trip-parser-arrivalair
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
title: arrivalAir
---
