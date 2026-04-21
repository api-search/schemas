---
description: ''
layout: schema
name: Location
properties_list:
- description: id of the ressource
  name: id
  type: string
- description: ''
  name: self
  type: object
- description: the resource name
  name: type
  type: string
- description: location sub type
  name: subType
  type: string
- description: short name of the location
  name: name
  type: string
- description: detailed name of the location. For a city location it contains city name and country code. For an airport location it contains city name; country code and airport full name
  name: detailedName
  type: string
- description: timezone offset of the location at the date of the API call (including daylight saving time)
  name: timeZoneOffset
  type: string
- description: IATA code of the location. ([IATA table codes](http://www.iata.org/publications/Pages/code-search.aspx) here)
  name: iataCode
  type: string
- description: ''
  name: geoCode
  type: object
- description: ''
  name: address
  type: object
- description: ''
  name: distance
  type: object
- description: ''
  name: analytics
  type: object
- description: score value calculated based on distance and analytics
  name: relevance
  type: number
- description: category of the location
  name: category
  type: string
- description: list of tags related to the location
  name: tags
  type: array
- description: the rank is the position compared to other locations based on how famous is a place. 1 being the highest.
  name: rank
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airport-city-search-location-schema.json
slug: airport-city-search-location
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
title: Location
---
