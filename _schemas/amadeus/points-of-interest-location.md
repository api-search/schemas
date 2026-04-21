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
- description: ''
  name: geoCode
  type: object
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
schema_file: json-schema/points-of-interest-location-schema.json
slug: points-of-interest-location
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
