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
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ConnectionRestriction\",\n  \"description\": \"Restriction towards number of connections.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxNumberOfConnections\": {\n      \"type\": \"number\",\n      \"description\": \"The maximal number of connections for each itinerary. Value can be 0, 1 or 2.\"\n    },\n    \"nonStopPreferred\": {\n      \"type\": \"boolean\",\n      \"description\": \"When this option is requested, recommendations made of Non-Stop flights only are favoured by the search, on the whole itinerary, with a weight of 75%. It is possible to override this default 75% weight of Non-Stop recommendations by providing the requested weight in the attribute nonStopPreferredWeight\"\n    },\n    \"nonStopPreferredWeight\": {\n      \"type\": \"number\",\n      \"description\": \"This weight is the percentage of total number of recommendations that could be returned for Non-Stop flight\
  \ recommendations. It is only relevant when combined with nonSTopPreferred set to true. If not specified, the default weight of 75% is applied\"\n    },\n    \"airportChangeAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Allow to change airport during connection\"\n    },\n    \"technicalStopsAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"This option allows the single segment to have one or more intermediate stops (technical stops).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-search-connectionrestriction-schema.json
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
