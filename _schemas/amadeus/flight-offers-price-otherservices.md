---
description: ''
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
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-offers-price-otherservices-schema.json
slug: flight-offers-price-otherservices
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"OtherServices\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"$ref\": \"#/definitions/ServiceName\"\n    },\n    \"price\": {\n      \"$ref\": \"#/definitions/ElementaryPrice\"\n    },\n    \"bookableByTraveler\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specify if the service is bookable by traveler or for all travelers\"\n    },\n    \"bookableByItinerary\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specify if the service is bookable by itinerary or for all itineraries\"\n    },\n    \"segmentIds\": {\n      \"type\": \"array\",\n      \"description\": \"Id of the segment concerned by the service\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"travelerIds\": {\n      \"type\": \"array\",\n      \"description\": \"Id of the traveler concerned by the service\",\n      \"items\": {\n        \"type\": \"string\"\
  \n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-offers-price-otherservices-schema.json
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
title: OtherServices
---
