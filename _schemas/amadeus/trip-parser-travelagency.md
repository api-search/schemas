---
description: details on the travel agency owning the trip
layout: schema
name: travelAgency
properties_list:
- description: Office name of the travel agency
  name: officeName
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: phone
  type: object
- description: ''
  name: email
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-travelagency-schema.json
slug: trip-parser-travelagency
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"travelAgency\",\n  \"description\": \"details on the travel agency owning the trip\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"officeName\": {\n      \"type\": \"string\",\n      \"description\": \"Office name of the travel agency\"\n    },\n    \"address\": {\n      \"$ref\": \"#/definitions/address\"\n    },\n    \"phone\": {\n      \"$ref\": \"#/definitions/phone\"\n    },\n    \"email\": {\n      \"$ref\": \"#/definitions/email\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-travelagency-schema.json
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
title: travelAgency
---
