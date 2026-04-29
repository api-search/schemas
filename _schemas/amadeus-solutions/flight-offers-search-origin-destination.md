---
description: OriginDestination schema
layout: schema
name: OriginDestination
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-search-origin-destination-schema.json
slug: flight-offers-search-origin-destination
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-origin-destination-schema.json\",\n  \"title\": \"OriginDestination\",\n  \"description\": \"OriginDestination schema\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/OriginDestinationLight\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"originRadius\": {\n          \"description\": \"Include other possible locations around the point, located less than this distance in kilometers away. Max:300\\n\\nCan not be combined with \\\"dateWindow\\\" or \\\"timeWindow\\\".\\n\",\n          \"type\": \"number\",\n          \"example\": 200\n        },\n        \"alternativeOriginsCodes\": {\n          \"type\": \"array\",\n          \"description\": \"Set of alternative origin location, such as a city or an airport. Currently, only the locations\
  \ defined in [IATA](http://www.iata.org/publications/Pages/code-search.aspx) are supported.\",\n          \"minItems\": 1,\n          \"maxItems\": 2,\n          \"items\": {\n            \"title\": \"code\",\n            \"type\": \"string\"\n          },\n          \"example\": [\n            \"LON\",\n            \"MUC\"\n          ]\n        },\n        \"destinationRadius\": {\n          \"description\": \"Include other possible locations around the point, located less than this distance in kilometers away. Max:300\\n\\nCan not be combined with \\\"dateWindow\\\" or \\\"timeWindow\\\".\\n\",\n          \"type\": \"number\",\n          \"example\": 200\n        },\n        \"alternativeDestinationsCodes\": {\n          \"type\": \"array\",\n          \"description\": \"Set of alternative destination location, such as a city or an airport. Currently, only the locations defined in [IATA](http://www.iata.org/publications/Pages/code-search.aspx) are supported.\",\n          \"minItems\"\
  : 1,\n          \"maxItems\": 2,\n          \"items\": {\n            \"title\": \"code\",\n            \"type\": \"string\"\n          }\n        },\n        \"departureDateTimeRange\": {\n          \"description\": \"Approximate date and time of departure, specified as a local date and time range.\",\n          \"$ref\": \"#/definitions/DateTimeRange\"\n        },\n        \"arrivalDateTimeRange\": {\n          \"description\": \"Approximate date and time of arrival, specified as a local date and time range.\",\n          \"$ref\": \"#/definitions/DateTimeRange\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-search-origin-destination-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: OriginDestination
---
