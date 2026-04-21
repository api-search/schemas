---
description: ''
layout: schema
name: Address
properties_list:
- description: name of the city of the location; equal to name if the location is a city
  name: cityName
  type: string
- description: IATA code of the city of the location; equal to IATAcode if the location is a city
  name: cityCode
  type: string
- description: name of the country of the location
  name: countryName
  type: string
- description: code of the country of the location in ISO standard
  name: countryCode
  type: string
- description: code of the state of the location if any
  name: stateCode
  type: string
- description: code of the region of the location in ISO standard
  name: regionCode
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airport-city-search-address-schema.json
slug: airport-city-search-address
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
