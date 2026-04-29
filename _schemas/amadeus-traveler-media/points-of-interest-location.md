---
description: Location schema
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
- description: category of the location
  name: category
  type: string
- description: list of tags related to the location
  name: tags
  type: array
- description: the rank is the position compared to other locations based on how famous is a place. 1 being the highest.
  name: rank
  type: string
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/points-of-interest-location-schema.json
slug: points-of-interest-location
source_filename: points-of-interest-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/points-of-interest-location-schema.json\",\n  \"title\": \"Location\",\n  \"description\": \"Location schema\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"id of the ressource\",\n      \"type\": \"string\"\n    },\n    \"self\": {\n      \"$ref\": \"#/definitions/Links\"\n    },\n    \"type\": {\n      \"description\": \"the resource name\",\n      \"type\": \"string\",\n      \"example\": \"location\"\n    },\n    \"subType\": {\n      \"description\": \"location sub type\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"AIRPORT\",\n        \"CITY\",\n        \"POINT_OF_INTEREST\",\n        \"DISTRICT\"\n      ],\n      \"example\": \"AIRPORT\"\n    },\n    \"name\": {\n      \"description\": \"short name of the location\",\n      \"type\": \"string\",\n      \"example\"\
  : \"Paris CDG\"\n    },\n    \"geoCode\": {\n      \"$ref\": \"#/definitions/GeoCode\"\n    },\n    \"category\": {\n      \"description\": \"category of the location\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"SIGHTS\",\n        \"BEACH_PARK\",\n        \"HISTORICAL\",\n        \"NIGHTLIFE\",\n        \"RESTAURANT\",\n        \"SHOPPING\"\n      ],\n      \"example\": \"HISTORICAL\"\n    },\n    \"tags\": {\n      \"description\": \"list of tags related to the location\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": [\n          \"grocery\",\n          \"japanese\",\n          \"cafe\"\n        ]\n      }\n    },\n    \"rank\": {\n      \"description\": \"the rank is the position compared to other locations based on how famous is a place. 1 being the highest.\",\n      \"type\": \"string\",\n      \"example\": 1\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/points-of-interest-location-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: Location
---
