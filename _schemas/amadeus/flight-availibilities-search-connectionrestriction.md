---
description: Restriction towards number of connections.
layout: schema
name: ConnectionRestriction
properties_list:
- description: The maximal number of connections for each itinerary. Value can be 0, 1 or 2.
  name: maxNumberOfConnections
  type: number
- description: Allow to change airport during connection
  name: airportChangeAllowed
  type: boolean
- description: This option allows the single segment to have one or more intermediate stops (technical stops).
  name: technicalStopsAllowed
  type: boolean
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-connectionrestriction-schema.json
slug: flight-availibilities-search-connectionrestriction
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
title: ConnectionRestriction
---
