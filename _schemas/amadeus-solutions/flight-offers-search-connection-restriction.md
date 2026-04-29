---
description: Restriction towards number of connections.
layout: schema
name: ConnectionRestriction
properties_list:
- description: The maximal number of connections for each itinerary. Value can be 0, 1 or 2.
  name: maxNumberOfConnections
  type: number
- description: When this option is requested, recommendations made of Non-Stop flights only are favoured by the search, on the whole itinerary, with a weight of 75%.
  name: nonStopPreferred
  type: boolean
- description: Allow to change airport during connection
  name: airportChangeAllowed
  type: boolean
- description: This option allows the single segment to have one or more intermediate stops (technical stops).
  name: technicalStopsAllowed
  type: boolean
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-connection-restriction-schema.json
slug: flight-offers-search-connection-restriction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-connection-restriction-schema.json\",\n  \"title\": \"ConnectionRestriction\",\n  \"description\": \"Restriction towards number of connections.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxNumberOfConnections\": {\n      \"description\": \"The maximal number of connections for each itinerary. Value can be 0, 1 or 2.\",\n      \"type\": \"number\",\n      \"example\": 2\n    },\n    \"nonStopPreferred\": {\n      \"description\": \"When this option is requested, recommendations made of Non-Stop flights only are favoured by the search, on the whole itinerary, with a weight of 75%.\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"airportChangeAllowed\": {\n      \"description\": \"Allow to change airport during connection\",\n      \"type\": \"\
  boolean\",\n      \"example\": false\n    },\n    \"technicalStopsAllowed\": {\n      \"description\": \"This option allows the single segment to have one or more intermediate stops (technical stops).\",\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-connection-restriction-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: ConnectionRestriction
---
