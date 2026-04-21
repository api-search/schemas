---
description: Restriction towards number of connections.
layout: schema
name: ConnectionRestriction
properties_list:
- description: The maximal number of connections for each itinerary. Value can be 0, 1 or 2.
  name: maxNumberOfConnections
  type: number
- description: When this option is requested, recommendations made of Non-Stop flights only are favoured by the search, on the whole itinerary, with a weight of 75%. It is possible to override this default 75% weigh
  name: nonStopPreferred
  type: boolean
- description: This weight is the percentage of total number of recommendations that could be returned for Non-Stop flight recommendations. It is only relevant when combined with nonSTopPreferred set to true. If not
  name: nonStopPreferredWeight
  type: number
- description: Allow to change airport during connection
  name: airportChangeAllowed
  type: boolean
- description: This option allows the single segment to have one or more intermediate stops (technical stops).
  name: technicalStopsAllowed
  type: boolean
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-search-connectionrestriction-schema.json
slug: flight-offers-search-connectionrestriction
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
