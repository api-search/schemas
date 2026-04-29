---
description: ''
layout: schema
name: FlightOffersSearchReply
properties_list:
- description: ''
  name: warnings
  type: array
- description: ''
  name: meta
  type: object
- description: ''
  name: data
  type: array
- description: ''
  name: dictionaries
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/flight-choice-prediction-flightofferssearchreply-schema.json
slug: flight-choice-prediction-flightofferssearchreply
source_filename: flight-choice-prediction-flightofferssearchreply-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"FlightOffersSearchReply\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"warnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Issue\"\n      }\n    },\n    \"meta\": {\n      \"$ref\": \"#/definitions/Collection_Meta\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/FlightOffer\"\n      }\n    },\n    \"dictionaries\": {\n      \"$ref\": \"#/definitions/Dictionaries\"\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/flight-choice-prediction-flightofferssearchreply-schema.json
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
title: FlightOffersSearchReply
---
