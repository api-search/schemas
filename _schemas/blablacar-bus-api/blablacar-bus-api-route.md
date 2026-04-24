---
description: A coach route between two stations in the BlaBlaCar Bus network
layout: schema
name: Route
properties_list:
- description: Unique route identifier
  name: id
  type: string
- description: Origin station identifier
  name: from_station_id
  type: string
- description: Destination station identifier
  name: to_station_id
  type: string
- description: Typical route duration in minutes
  name: duration_minutes
  type: integer
- description: Route distance in kilometers
  name: distance_km
  type: integer
provider_name: BlaBlaCar Bus API
provider_slug: blablacar-bus-api
schema_file: json-schema/blablacar-bus-api-route-schema.json
slug: blablacar-bus-api-route
tags:
- Booking
- Buses
- Coach
- Europe
- Mobility
- Ticketing
- Transportation
- Travel
title: Route
---
