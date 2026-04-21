---
description: address information
layout: schema
name: Address
properties_list:
- description: Address line with street, number, bulding, etc...
  name: line
  type: string
- description: Post office code number
  name: zip
  type: string
- description: Country code (two character standard IATA country code)
  name: countryCode
  type: string
- description: City, town or postal station
  name: cityName
  type: string
- description: State code (two character standard IATA state code)
  name: stateCode
  type: string
- description: latitude of the location
  name: latitude
  type: number
- description: longitude of the location
  name: longitude
  type: number
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-search-address-schema.json
slug: transfer-search-address
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
title: Address
---
