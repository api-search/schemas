---
description: A point of interest returned by the Foursquare Places API.
layout: schema
name: FoursquarePlace
properties_list:
- description: Stable Foursquare place identifier.
  name: fsq_id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: location
  type: object
- description: ''
  name: geocodes
  type: object
- description: ''
  name: categories
  type: array
- description: ''
  name: chains
  type: array
- description: ''
  name: distance
  type: integer
- description: ''
  name: rating
  type: number
- description: ''
  name: popularity
  type: number
- description: ''
  name: verified
  type: boolean
provider_name: Foursquare
provider_slug: foursquare
schema_file: json-schema/foursquare-place.json
slug: foursquare-place
source_filename: foursquare-place.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/json-schema/foursquare-place.json\",\n  \"title\": \"FoursquarePlace\",\n  \"description\": \"A point of interest returned by the Foursquare Places API.\",\n  \"type\": \"object\",\n  \"required\": [\"fsq_id\", \"name\"],\n  \"properties\": {\n    \"fsq_id\": { \"type\": \"string\", \"description\": \"Stable Foursquare place identifier.\" },\n    \"name\": { \"type\": \"string\" },\n    \"location\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"address\": { \"type\": \"string\" },\n        \"locality\": { \"type\": \"string\" },\n        \"region\": { \"type\": \"string\" },\n        \"postcode\": { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\" },\n        \"formatted_address\": { \"type\": \"string\" }\n      }\n    },\n    \"geocodes\": {\n      \"type\": \"object\",\n   \
  \   \"properties\": {\n        \"main\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"latitude\": { \"type\": \"number\" },\n            \"longitude\": { \"type\": \"number\" }\n          }\n        }\n      }\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"integer\" },\n          \"name\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"chains\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"string\" },\n          \"name\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"distance\": { \"type\": \"integer\" },\n    \"rating\": { \"type\": \"number\" },\n    \"popularity\": { \"type\": \"number\" },\n    \"verified\": { \"type\": \"boolean\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/foursquare/refs/heads/main/json-schema/foursquare-place.json
tags:
- Locations
- Places
- Geocoding
- Recommendations
- Reviews
- Movement
title: FoursquarePlace
---
