---
description: A coach station in the BlaBlaCar Bus network
layout: schema
name: Station
properties_list:
- description: Unique station identifier
  name: id
  type: string
- description: Station name
  name: name
  type: string
- description: City where the station is located
  name: city
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: country_code
  type: string
- description: Geographic latitude
  name: latitude
  type: number
- description: Geographic longitude
  name: longitude
  type: number
- description: Full street address
  name: address
  type: string
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
schema_file: json-schema/blablacar-bus-api-station-schema.json
slug: blablacar-bus-api-station
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
title: Station
---
