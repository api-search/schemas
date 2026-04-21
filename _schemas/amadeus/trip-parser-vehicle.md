---
description: Vehicle describes the transportation means e.g. a Train, a Bus, etc. It may be further characterized, in the case of a Train, it contains the Train Number, Code etc.
layout: schema
name: vehicle
properties_list:
- description: Code (codelist TVT) for the generic transport service returned, e.g. High speed, Intercities, Night and so on
  name: vehicleType
  type: string
- description: ''
  name: code
  type: string
- description: ''
  name: number
  type: string
- description: ''
  name: displayName
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-vehicle-schema.json
slug: trip-parser-vehicle
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
title: vehicle
---
