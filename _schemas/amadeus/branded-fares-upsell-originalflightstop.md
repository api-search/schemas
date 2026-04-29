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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/branded-fares-upsell-originalflightstop-schema.json
slug: branded-fares-upsell-originalflightstop
source_filename: branded-fares-upsell-originalflightstop-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"OriginalFlightStop\",\n  \"description\": \"details of stops for direct or change of gauge flights\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"[IATA airline codes](http://www.iata.org/publications/Pages/code-search.aspx)\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"stop duration in [ISO8601](https://en.wikipedia.org/wiki/ISO_8601) PnYnMnDTnHnMnS format, e.g. PT2H10M\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/branded-fares-upsell-originalflightstop-schema.json
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
title: OriginalFlightStop
---
