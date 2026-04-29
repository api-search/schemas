---
description: checked bag
layout: schema
name: Bags
properties_list: []
provider_name: Amadeus Solutions
provider_slug: amadeus-solutions
schema_file: json-schema/flight-offers-price-bags-schema.json
slug: flight-offers-price-bags
source_filename: flight-offers-price-bags-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-bags-schema.json\",\n  \"title\": \"Bags\",\n  \"description\": \"checked bag\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/definitions/BaggageAllowance\"\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"description\": \"Type of service\",\n          \"type\": \"string\",\n          \"example\": \"CHECKED_BAG\"\n        },\n        \"price\": {\n          \"$ref\": \"#/definitions/ElementaryPrice\"\n        },\n        \"bookableByItinerary\": {\n          \"description\": \"Specify if the service is bookable by itinerary  or for all itineraries\",\n          \"type\": \"boolean\",\n          \"example\": false\n        },\n        \"segmentIds\": {\n          \"description\": \"Id of the segment concerned by the service\",\n\
  \          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"example\": \"1\"\n        },\n        \"travelerIds\": {\n          \"description\": \"Id of the traveler concerned by the service\",\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"example\": \"1\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-solutions/refs/heads/main/json-schema/flight-offers-price-bags-schema.json
tags:
- Airlines
- Booking
- Flights
- GDS
- Hotels
- Travel
- Travel Technology
title: Bags
---
