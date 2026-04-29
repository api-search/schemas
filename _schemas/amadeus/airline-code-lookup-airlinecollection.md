---
description: A collection response containing an array of airline resources and associated metadata.
layout: schema
name: AirlineCollection
properties_list:
- description: ''
  name: meta
  type: object
- description: Array of airline resources matching the query.
  name: data
  type: array
- description: Non-blocking issues encountered during the request processing.
  name: warnings
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-code-lookup-airlinecollection-schema.json
slug: airline-code-lookup-airlinecollection
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AirlineCollection\",\n  \"description\": \"A collection response containing an array of airline resources and associated metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"meta\": {\n      \"$ref\": \"#/definitions/CollectionMeta\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of airline resources matching the query.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Airline\"\n      }\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"description\": \"Non-blocking issues encountered during the request processing.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airline-code-lookup-airlinecollection-schema.json
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
title: AirlineCollection
---
