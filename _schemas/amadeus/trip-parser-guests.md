---
description: ''
layout: schema
name: guests
properties_list:
- description: number of adult guests (1-9) per room
  name: adults
  type: integer
- description: Comma separated list of ages of each child at the time of check-out from the hotel. If several children have the same age, the ages will be repeated.
  name: childAge
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-guests-schema.json
slug: trip-parser-guests
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
title: guests
---
