---
description: ''
layout: schema
name: Location
properties_list:
- description: id of the ressource
  name: id
  type: string
- description: ''
  name: self
  type: object
- description: the resource name
  name: type
  type: string
- description: location sub type
  name: subType
  type: string
- description: short name of the location
  name: name
  type: string
- description: ''
  name: geoCode
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/safe-place-location-schema.json
slug: safe-place-location
source_filename: safe-place-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Location\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"id of the ressource\"\n    },\n    \"self\": {\n      \"$ref\": \"#/definitions/Links\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\"\n    },\n    \"subType\": {\n      \"type\": \"string\",\n      \"description\": \"location sub type\",\n      \"enum\": [\n        \"AIRPORT\",\n        \"CITY\",\n        \"POINT_OF_INTEREST\",\n        \"DISTRICT\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"short name of the location\"\n    },\n    \"geoCode\": {\n      \"$ref\": \"#/definitions/GeoCode\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/safe-place-location-schema.json
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
title: Location
---
