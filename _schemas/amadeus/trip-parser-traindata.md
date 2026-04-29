---
description: Train Product
layout: schema
name: trainData
properties_list:
- description: Confirmation number
  name: confirmNbr
  type: string
- description: Provider name
  name: serviceProviderName
  type: string
- description: Booking class
  name: bookingClass
  type: string
- description: ''
  name: departure
  type: object
- description: Date in ISO 8601 (http://www.w3.org/TR/NOTE-datetime), YYYY-MM-DDTHH:MM:SSZ.
  name: departureDateTime
  type: string
- description: Date in ISO 8601 (http://www.w3.org/TR/NOTE-datetime), YYYY-MM-DDTHH:MM:SSZ.
  name: arrivalDateTime
  type: string
- description: ''
  name: arrival
  type: object
- description: Duration in ISO 8601 / RFC 3339 (https://www.ietf.org/rfc/rfc3339.txt), P[n]Y[n]M[n]DT[n]H[n]M[n]S.
  name: duration
  type: string
- description: ''
  name: departureTrack
  type: string
- description: ''
  name: arrivalTrack
  type: string
- description: ''
  name: seats
  type: array
- description: ''
  name: vehicle
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/trip-parser-traindata-schema.json
slug: trip-parser-traindata
source_filename: trip-parser-traindata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"trainData\",\n  \"description\": \"Train Product\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"confirmNbr\": {\n      \"type\": \"string\",\n      \"description\": \"Confirmation number\"\n    },\n    \"serviceProviderName\": {\n      \"type\": \"string\",\n      \"description\": \"Provider name\"\n    },\n    \"bookingClass\": {\n      \"type\": \"string\",\n      \"description\": \"Booking class\"\n    },\n    \"departure\": {\n      \"$ref\": \"#/definitions/departure\"\n    },\n    \"departureDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date in ISO 8601 (http://www.w3.org/TR/NOTE-datetime), YYYY-MM-DDTHH:MM:SSZ.\"\n    },\n    \"arrivalDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date in ISO 8601 (http://www.w3.org/TR/NOTE-datetime), YYYY-MM-DDTHH:MM:SSZ.\"\n    },\n    \"arrival\": {\n      \"$ref\": \"#/definitions/arrival\"\n    },\n\
  \    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"Duration in ISO 8601 / RFC 3339 (https://www.ietf.org/rfc/rfc3339.txt), P[n]Y[n]M[n]DT[n]H[n]M[n]S.\"\n    },\n    \"departureTrack\": {\n      \"type\": \"string\"\n    },\n    \"arrivalTrack\": {\n      \"type\": \"string\"\n    },\n    \"seats\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/seats\"\n      }\n    },\n    \"vehicle\": {\n      \"$ref\": \"#/definitions/vehicle\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/trip-parser-traindata-schema.json
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
title: trainData
---
