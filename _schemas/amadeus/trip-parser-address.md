---
description: Address information
layout: schema
name: address
properties_list:
- description: Category of the contact element
  name: category
  type: string
- description: Line 1 = Street address, Line 2 = Apartment, suite, unit, building, floor, etc
  name: lines
  type: array
- description: 'Example: 74130'
  name: postalCode
  type: string
- description: ISO 3166-1 country code
  name: countryCode
  type: string
- description: 'Full city name. Example: Dublin'
  name: cityName
  type: string
- description: State code (two character standard IATA state code)
  name: stateCode
  type: string
- description: E.g. BP 220
  name: postalBox
  type: string
- description: Field containing a full unformatted address. Only applicable when the fields lines, postalCode, countryCode, cityName are not filled.
  name: text
  type: string
- description: State, province or country name
  name: state
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-address-schema.json
slug: trip-parser-address
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
title: address
---
