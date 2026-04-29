---
description: price metric
layout: schema
name: itinerary-price-metric
properties_list:
- description: ressource type - always price-metrics
  name: type
  type: string
- description: Description of a particular point or place in physical space
  name: origin
  type: object
- description: Description of a particular point or place in physical space
  name: destination
  type: object
- description: The date on which the traveler will depart from the origin to go to the destination. Dates are specified in the[ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-DD format.
  name: departureDate
  type: string
- description: transportation type
  name: transportType
  type: string
- description: currency of the prices. Currency is specified in the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) format, e.g. EUR for Euro
  name: currencyCode
  type: string
- description: true for a one way trip, false for a round trip
  name: oneWay
  type: boolean
- description: ''
  name: priceMetrics
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-price-analysis-itinerary-price-metric-schema.json
slug: flight-price-analysis-itinerary-price-metric
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"itinerary-price-metric\",\n  \"description\": \"price metric\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"ressource type - always price-metrics\"\n    },\n    \"origin\": {\n      \"type\": \"object\",\n      \"description\": \"Description of a particular point or place in physical space\",\n      \"properties\": {\n        \"iataCode\": {\n          \"type\": \"string\",\n          \"description\": \"IATA location code\"\n        }\n      }\n    },\n    \"destination\": {\n      \"type\": \"object\",\n      \"description\": \"Description of a particular point or place in physical space\",\n      \"properties\": {\n        \"iataCode\": {\n          \"type\": \"string\",\n          \"description\": \"IATA location code\"\n        }\n      }\n    },\n    \"departureDate\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The date on which the traveler will depart from the origin to go to the destination. \\n\\nDates are specified in the[ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) YYYY-MM-DD format.\"\n    },\n    \"transportType\": {\n      \"type\": \"string\",\n      \"description\": \"transportation type\",\n      \"enum\": [\n        \"FLIGHT\"\n      ]\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"currency of the prices.\\n\\nCurrency is specified in the [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) format, e.g. EUR for Euro\"\n    },\n    \"oneWay\": {\n      \"type\": \"boolean\",\n      \"description\": \"true for a one way trip,\\nfalse for a round trip\"\n    },\n    \"priceMetrics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"amount\": {\n            \"type\": \"string\",\n            \"description\": \"Defines the monetary value with decimal position. It can\
  \ be in cash or miles.\"\n          },\n          \"quartileRanking\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"MINIMUM\",\n              \"FIRST\",\n              \"MEDIUM\",\n              \"THIRD\",\n              \"MAXIMUM\"\n            ]\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-price-analysis-itinerary-price-metric-schema.json
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
title: itinerary-price-metric
---
