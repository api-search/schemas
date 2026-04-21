---
description: ''
layout: schema
name: GetFlightAvailabilitiesQuery
properties_list:
- description: 'Origins and Destinations must be properly ordered in time (chronological order in accordance with the timezone of each location) to describe the journey consistently. Dates and times must not be past '
  name: originDestinations
  type: array
- description: List of travelers composing the travel
  name: travelers
  type: array
- description: 'Allows enable one or more sources. If present in the list, these sources will be called by the system. GDS : Full service carriers'
  name: sources
  type: array
- description: ''
  name: searchCriteria
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-getflightavailabilitiesquery-schema.json
slug: flight-availibilities-search-getflightavailabilitiesquery
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
title: GetFlightAvailabilitiesQuery
---
