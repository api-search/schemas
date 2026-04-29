---
description: OriginDestinationLight schema
layout: schema
name: OriginDestinationLight
properties_list:
- description: ''
  name: id
  type: string
- description: Origin location, such as a city or an airport. Currently, only the locations defined in [IATA](http://www.iata.org/publications/Pages/code-search.aspx) are supported.
  name: originLocationCode
  type: string
- description: Destination location, such as a city or an airport. Currently, only the locations defined in [IATA](http://www.iata.org/publications/Pages/code-search.aspx) are supported.
  name: destinationLocationCode
  type: string
- description: List of included connections points. When an includedViaPoints option is specified, all FlightOffer returned must at least go via this Connecting Point. Currently, only the locations defined in IATA a
  name: includedConnectionPoints
  type: array
- description: List of excluded connections points. Any FlightOffer with these connections points will be present in response. Currently, only the locations defined in IATA are supported. Used only by the AMADEUS pr
  name: excludedConnectionPoints
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-origin-destination-light-schema.json
slug: flight-offers-search-origin-destination-light
source_filename: flight-offers-search-origin-destination-light-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-origin-destination-light-schema.json\",\n  \"title\": \"OriginDestinationLight\",\n  \"description\": \"OriginDestinationLight schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": 1\n    },\n    \"originLocationCode\": {\n      \"description\": \"Origin location, such as a city or an airport. Currently, only the locations defined in [IATA](http://www.iata.org/publications/Pages/code-search.aspx) are supported.\",\n      \"type\": \"string\",\n      \"example\": \"PAR\"\n    },\n    \"destinationLocationCode\": {\n      \"description\": \"Destination location, such as a city or an airport. Currently, only the locations defined in [IATA](http://www.iata.org/publications/Pages/code-search.aspx) are supported.\",\n  \
  \    \"type\": \"string\",\n      \"example\": \"NYC\"\n    },\n    \"includedConnectionPoints\": {\n      \"type\": \"array\",\n      \"description\": \"List of included connections points. When an includedViaPoints option is specified, all FlightOffer returned must at least go via this Connecting Point. Currently, only the locations defined in IATA are supported. Used only by the AMADEUS provider\",\n      \"minItems\": 1,\n      \"maxItems\": 2,\n      \"items\": {\n        \"title\": \"code\",\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"MRS\"\n      ]\n    },\n    \"excludedConnectionPoints\": {\n      \"type\": \"array\",\n      \"description\": \"List of excluded connections points. Any FlightOffer with these connections points will be present in response. Currently, only the locations defined in IATA are supported. Used only by the AMADEUS provider\",\n      \"minItems\": 1,\n      \"maxItems\": 3,\n      \"items\": {\n        \"title\": \"code\",\n\
  \        \"type\": \"string\"\n      },\n      \"example\": [\n        \"MRS\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-origin-destination-light-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: OriginDestinationLight
---
