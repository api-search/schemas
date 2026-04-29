---
description: ''
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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-origindestinationlight-schema.json
slug: flight-availibilities-search-origindestinationlight
source_filename: flight-availibilities-search-origindestinationlight-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"OriginDestinationLight\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"originLocationCode\": {\n      \"type\": \"string\",\n      \"description\": \"Origin location, such as a city or an airport. Currently, only the locations defined in [IATA](http://www.iata.org/publications/Pages/code-search.aspx) are supported.\"\n    },\n    \"destinationLocationCode\": {\n      \"type\": \"string\",\n      \"description\": \"Destination location, such as a city or an airport. Currently, only the locations defined in [IATA](http://www.iata.org/publications/Pages/code-search.aspx) are supported.\"\n    },\n    \"includedConnectionPoints\": {\n      \"type\": \"array\",\n      \"description\": \"List of included connections points. When an includedViaPoints option is specified, all FlightOffer returned must at least go via this Connecting Point. Currently,\
  \ only the locations defined in IATA are supported. Used only by the AMADEUS provider\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"excludedConnectionPoints\": {\n      \"type\": \"array\",\n      \"description\": \"List of excluded connections points. Any FlightOffer with these connections points will be present in response. Currently, only the locations defined in IATA are supported. Used only by the AMADEUS provider\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-availibilities-search-origindestinationlight-schema.json
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
title: OriginDestinationLight
---
