---
description: Description of a particular point or place in physical space
layout: schema
name: end
properties_list:
- description: Local Date/Time of the itinerary end in format ISO 8601 (YYYY-MM-DDTHH:MM:SS)
  name: localDateTime
  type: string
- description: Label associated to the location (e.g. Eiffel Tower, Madison Square)
  name: name
  type: string
- description: IATA location code
  name: iataCode
  type: string
- description: ''
  name: address
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-end-schema.json
slug: trip-parser-end
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
title: end
---
