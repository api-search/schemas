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
- description: detailed name of the location. For a city location it contains city name and country code. For an airport location it contains city name; country code and airport full name
  name: detailedName
  type: string
- description: timezone offset of the location at the date of the API call (including daylight saving time)
  name: timeZoneOffset
  type: string
- description: IATA code of the location. ([IATA table codes](http://www.iata.org/publications/Pages/code-search.aspx) here)
  name: iataCode
  type: string
- description: ''
  name: geoCode
  type: object
- description: ''
  name: address
  type: object
- description: ''
  name: distance
  type: object
- description: ''
  name: analytics
  type: object
- description: score value calculated based on distance and analytics
  name: relevance
  type: number
- description: category of the location
  name: category
  type: string
- description: list of tags related to the location
  name: tags
  type: array
- description: the rank is the position compared to other locations based on how famous is a place. 1 being the highest.
  name: rank
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airport-city-search-location-schema.json
slug: airport-city-search-location
source_filename: airport-city-search-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Location\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"id of the ressource\"\n    },\n    \"self\": {\n      \"$ref\": \"#/definitions/Links\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"the resource name\"\n    },\n    \"subType\": {\n      \"type\": \"string\",\n      \"description\": \"location sub type\",\n      \"enum\": [\n        \"AIRPORT\",\n        \"CITY\",\n        \"POINT_OF_INTEREST\",\n        \"DISTRICT\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"short name of the location\"\n    },\n    \"detailedName\": {\n      \"type\": \"string\",\n      \"description\": \"detailed name of the location. For a city location it contains city name and country code. For an airport location it contains city name; country code and airport full name\"\
  \n    },\n    \"timeZoneOffset\": {\n      \"type\": \"string\",\n      \"description\": \"timezone offset of the location at the date of the API call (including daylight saving time)\"\n    },\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"IATA code of the location. ([IATA table codes](http://www.iata.org/publications/Pages/code-search.aspx) here)\"\n    },\n    \"geoCode\": {\n      \"$ref\": \"#/definitions/GeoCode\"\n    },\n    \"address\": {\n      \"$ref\": \"#/definitions/Address\"\n    },\n    \"distance\": {\n      \"$ref\": \"#/definitions/Distance\"\n    },\n    \"analytics\": {\n      \"$ref\": \"#/definitions/Analytics\"\n    },\n    \"relevance\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"score value calculated based on distance and analytics\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"category of the location\",\n      \"enum\": [\n        \"SIGHTS\",\n \
  \       \"BEACH_PARK\",\n        \"HISTORICAL\",\n        \"NIGHTLIFE\",\n        \"RESTAURANT\",\n        \"SHOPPING\"\n      ]\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"list of tags related to the location\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"rank\": {\n      \"type\": \"string\",\n      \"description\": \"the rank is the position compared to other locations based on how famous is a place. 1 being the highest.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airport-city-search-location-schema.json
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
