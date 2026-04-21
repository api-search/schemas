---
description: Meta information about the returned object(s) in "data"
layout: schema
name: Meta
properties_list:
- description: Total number of object(s) retrieved
  name: count
  type: integer
- description: Sorting fields criteria and their associated priority and direction. Sorting priority is indicated by the order of the strings within the array. E.g. sort=title,size means that items are ordered by ti
  name: sort
  type: array
- description: Links related to the returned object(s)
  name: links
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-list-meta-schema.json
slug: hotel-list-meta
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
title: Meta
---
