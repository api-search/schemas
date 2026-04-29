---
description: ''
layout: schema
name: GeneralRemark
properties_list:
- description: ''
  name: subType
  type: object
- description: remark category
  name: category
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
schema_file: json-schema/flight-create-orders-generalremark-schema.json
slug: flight-create-orders-generalremark
source_filename: flight-create-orders-generalremark-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"GeneralRemark\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subType\": {\n      \"$ref\": \"#/definitions/GeneralRemarkType\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"remark category\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"remark free text\"\n    },\n    \"travelerIds\": {\n      \"type\": \"array\",\n      \"description\": \"Id of the concerned traveler\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"flightOfferIds\": {\n      \"type\": \"array\",\n      \"description\": \"Id of the concern flightOffers\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"subType\",\n    \"text\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-create-orders-generalremark-schema.json
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
title: GeneralRemark
---
