---
description: Location of the stop over or the several stop over points. It can be defined either using IATA code or Address (address line, zip, country, city, state, latitude, longitude, lfi). Vehicle change via stop overs is not supported.
layout: schema
name: StopOver
properties_list:
- description: transfer stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M.
  name: duration
  type: string
- description: sequence number of the stop e.g. 3
  name: sequenceNumber
  type: number
- description: ''
  name: location
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/transfer-search-stopover-schema.json
slug: transfer-search-stopover
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"StopOver\",\n  \"description\": \"Location of the stop over or the several stop over points. It can be defined either using IATA code or Address (address line, zip, country, city, state, latitude, longitude, lfi). Vehicle change via stop overs is not supported.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"transfer stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M.\"\n    },\n    \"sequenceNumber\": {\n      \"type\": \"number\",\n      \"description\": \"sequence number of the stop e.g. 3\"\n    },\n    \"location\": {\n      \"$ref\": \"#/definitions/Location\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/transfer-search-stopover-schema.json
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
title: StopOver
---
