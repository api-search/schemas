---
description: Activity description
layout: schema
name: Activity
properties_list:
- description: the ressource name
  name: type
  type: string
- description: unique id of the ressource
  name: id
  type: string
- description: ''
  name: self
  type: object
- description: activity name
  name: name
  type: string
- description: short description of the activity
  name: shortDescription
  type: string
- description: full description of the activity
  name: description
  type: string
- description: ''
  name: geoCode
  type: object
- description: rating of the activity
  name: rating
  type: string
- description: ''
  name: price
  type: object
- description: link to picture related to the activity
  name: pictures
  type: array
- description: url to book the activity
  name: bookingLink
  type: string
- description: Minimum recommended duration for the activity
  name: minimumDuration
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/tours-and-activities-activity-schema.json
slug: tours-and-activities-activity
source_filename: tours-and-activities-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Activity\",\n  \"description\": \"Activity description\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the ressource name\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"unique id of the ressource\"\n    },\n    \"self\": {\n      \"$ref\": \"#/definitions/Link\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"activity name\"\n    },\n    \"shortDescription\": {\n      \"type\": \"string\",\n      \"description\": \"short description of the activity\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"full description of the activity\"\n    },\n    \"geoCode\": {\n      \"$ref\": \"#/definitions/GeoCode\"\n    },\n    \"rating\": {\n      \"type\": \"string\",\n      \"description\": \"rating of the activity\"\n    },\n    \"\
  price\": {\n      \"$ref\": \"#/definitions/ElementaryPrice\"\n    },\n    \"pictures\": {\n      \"type\": \"array\",\n      \"description\": \"link to picture related to the activity\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"bookingLink\": {\n      \"type\": \"string\",\n      \"description\": \"url to book the activity\"\n    },\n    \"minimumDuration\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum recommended duration for the activity\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/tours-and-activities-activity-schema.json
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
title: Activity
---
