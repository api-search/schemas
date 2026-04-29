---
description: ''
layout: schema
name: AirlineRemark
properties_list:
- description: ''
  name: subType
  type: object
- description: keyword code - only applicable for subType Keyword
  name: keyword
  type: string
- description: Code of the airline following IATA standard ([IATA table codes](http://www.iata.org/publications/Pages/code-search.aspx)) When it apply to any airline, value is YY.
  name: airlineCode
  type: string
- description: remark free text
  name: text
  type: string
- description: Id of the concerned traveler
  name: travelerIds
  type: array
- description: Id of the concern flightOffers
  name: flightOfferIds
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-create-orders-airlineremark-schema.json
slug: flight-create-orders-airlineremark
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AirlineRemark\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subType\": {\n      \"$ref\": \"#/definitions/AirlineRemarkType\"\n    },\n    \"keyword\": {\n      \"type\": \"string\",\n      \"description\": \"keyword code - only applicable for subType Keyword\"\n    },\n    \"airlineCode\": {\n      \"type\": \"string\",\n      \"description\": \"Code of the airline following IATA standard ([IATA table codes](http://www.iata.org/publications/Pages/code-search.aspx))\\n\\nWhen it apply to any airline, value is YY.\\n\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"remark free text\"\n    },\n    \"travelerIds\": {\n      \"type\": \"array\",\n      \"description\": \"Id of the concerned traveler\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"flightOfferIds\": {\n      \"type\": \"array\",\n      \"description\": \"Id of the\
  \ concern flightOffers\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"subType\",\n    \"airlineCode\",\n    \"text\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-create-orders-airlineremark-schema.json
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
title: AirlineRemark
---
