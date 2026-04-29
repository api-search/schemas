---
description: ''
layout: schema
name: SearchCriteriaLight
properties_list:
- description: This option allows to exclude the isAllotment flag associated to a booking class in the search response when it exist.
  name: excludeAllotments
  type: boolean
- description: ''
  name: flightFilters
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-availibilities-search-searchcriterialight-schema.json
slug: flight-availibilities-search-searchcriterialight
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"SearchCriteriaLight\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"excludeAllotments\": {\n      \"type\": \"boolean\",\n      \"description\": \"This option allows to exclude the isAllotment flag associated to a booking class in the search response when it exist.\"\n    },\n    \"flightFilters\": {\n      \"$ref\": \"#/definitions/FlightFiltersLight\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-availibilities-search-searchcriterialight-schema.json
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
title: SearchCriteriaLight
---
