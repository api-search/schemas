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
source_filename: flight-availibilities-search-connectionrestriction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ConnectionRestriction\",\n  \"description\": \"Restriction towards number of connections.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxNumberOfConnections\": {\n      \"type\": \"number\",\n      \"description\": \"The maximal number of connections for each itinerary. Value can be 0, 1 or 2.\"\n    },\n    \"airportChangeAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Allow to change airport during connection\"\n    },\n    \"technicalStopsAllowed\": {\n      \"type\": \"boolean\",\n      \"description\": \"This option allows the single segment to have one or more intermediate stops (technical stops).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-availibilities-search-connectionrestriction-schema.json
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
