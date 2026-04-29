---
description: AirlineRemark schema
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
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-create-orders-airline-remark-schema.json
slug: flight-create-orders-airline-remark
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-airline-remark-schema.json\",\n  \"title\": \"AirlineRemark\",\n  \"description\": \"AirlineRemark schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subType\": {\n      \"$ref\": \"#/definitions/AirlineRemarkType\"\n    },\n    \"keyword\": {\n      \"description\": \"keyword code - only applicable for subType Keyword\",\n      \"type\": \"string\",\n      \"example\": \"PARK\"\n    },\n    \"airlineCode\": {\n      \"description\": \"Code of the airline following IATA standard ([IATA table codes](http://www.iata.org/publications/Pages/code-search.aspx))\\n\\nWhen it apply to any airline, value is YY.\\n\",\n      \"type\": \"string\",\n      \"example\": \"AF\"\n    },\n    \"text\": {\n      \"description\": \"remark free text\",\n      \"type\": \"string\",\n \
  \     \"example\": \"CAR PARK\"\n    },\n    \"travelerIds\": {\n      \"description\": \"Id of the concerned traveler\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    },\n    \"flightOfferIds\": {\n      \"description\": \"Id of the concern flightOffers\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    }\n  },\n  \"required\": [\n    \"subType\",\n    \"airlineCode\",\n    \"text\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-create-orders-airline-remark-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: AirlineRemark
---
