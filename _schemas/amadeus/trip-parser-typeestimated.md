---
description: estimated room category, bed type and number of beds in the room. This information has been parsed from the room description, and is thus only provided for informational purposes
layout: schema
name: typeEstimated
properties_list:
- description: Category code
  name: category
  type: string
- description: Number of beds in the room (1-9)
  name: beds
  type: integer
- description: Type of the bed
  name: bedType
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-typeestimated-schema.json
slug: trip-parser-typeestimated
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
title: typeEstimated
---
