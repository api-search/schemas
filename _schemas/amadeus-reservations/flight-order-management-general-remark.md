---
description: GeneralRemark schema
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
provider_name: Amadeus Reservations
provider_slug: amadeus-reservations
schema_file: json-schema/flight-order-management-general-remark-schema.json
slug: flight-order-management-general-remark
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-general-remark-schema.json\",\n  \"title\": \"GeneralRemark\",\n  \"description\": \"GeneralRemark schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subType\": {\n      \"$ref\": \"#/definitions/GeneralRemarkType\"\n    },\n    \"category\": {\n      \"description\": \"remark category\",\n      \"type\": \"string\",\n      \"example\": \"Z\",\n      \"pattern\": \"[A-Z]{1}\"\n    },\n    \"text\": {\n      \"description\": \"remark free text\",\n      \"type\": \"string\",\n      \"example\": \"PASSENGER NEED ASSISTANCE\"\n    },\n    \"travelerIds\": {\n      \"description\": \"Id of the concerned traveler\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    },\n    \"flightOfferIds\": {\n  \
  \    \"description\": \"Id of the concern flightOffers\",\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"maxItems\": 6,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    }\n  },\n  \"required\": [\n    \"subType\",\n    \"text\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-reservations/refs/heads/main/json-schema/flight-order-management-general-remark-schema.json
tags:
- Booking
- Flights
- Hotels
- Reservations
- Travel
title: GeneralRemark
---
