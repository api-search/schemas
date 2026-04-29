---
description: OtherServices schema
layout: schema
name: OtherServices
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: price
  type: object
- description: Specify if the service is bookable by traveler or for all travelers
  name: bookableByTraveler
  type: boolean
- description: Specify if the service is bookable by itinerary or for all itineraries
  name: bookableByItinerary
  type: boolean
- description: Id of the segment concerned by the service
  name: segmentIds
  type: array
- description: Id of the traveler concerned by the service
  name: travelerIds
  type: array
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-other-services-schema.json
slug: flight-offers-price-other-services
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-other-services-schema.json\",\n  \"title\": \"OtherServices\",\n  \"description\": \"OtherServices schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"$ref\": \"#/definitions/ServiceName\"\n    },\n    \"price\": {\n      \"$ref\": \"#/definitions/ElementaryPrice\"\n    },\n    \"bookableByTraveler\": {\n      \"description\": \"Specify if the service is bookable by traveler or for all travelers\",\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"bookableByItinerary\": {\n      \"description\": \"Specify if the service is bookable by itinerary or for all itineraries\",\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"segmentIds\": {\n      \"description\": \"Id of the segment concerned by the service\",\n   \
  \   \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    },\n    \"travelerIds\": {\n      \"description\": \"Id of the traveler concerned by the service\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": \"1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-other-services-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: OtherServices
---
