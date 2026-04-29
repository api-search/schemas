---
description: details of stops for direct or change of gauge flights
layout: schema
name: OriginalFlightStop
properties_list:
- description: '[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)'
  name: iataCode
  type: string
- description: stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M
  name: duration
  type: string
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-original-flight-stop-schema.json
slug: flight-offers-price-original-flight-stop
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-original-flight-stop-schema.json\",\n  \"title\": \"OriginalFlightStop\",\n  \"description\": \"details of stops for direct or change of gauge flights\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataCode\": {\n      \"description\": \"[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)\",\n      \"type\": \"string\",\n      \"example\": \"JFK\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M\",\n      \"example\": \"PT2H10M\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-original-flight-stop-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: OriginalFlightStop
---
