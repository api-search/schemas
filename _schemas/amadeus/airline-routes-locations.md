---
description: Description of a particular point or place in physical space
layout: schema
name: locations
properties_list:
- description: type of API result "location"
  name: type
  type: string
- description: Location sub-type (e.g. airport, port, rail-station, restaurant, atm...)
  name: subtype
  type: string
- description: Label associated to the location (e.g. Eiffel Tower, Madison Square)
  name: name
  type: string
- description: IATA location code
  name: iataCode
  type: string
- description: Geographic coordinates describing the position of any location on the surface of Earth
  name: geoCode
  type: object
- description: ''
  name: address
  type: object
- description: ''
  name: timeZone
  type: object
- description: ''
  name: metrics
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/airline-routes-locations-schema.json
slug: airline-routes-locations
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"locations\",\n  \"description\": \"Description of a particular point or place in physical space\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"type of API result \\\"location\\\"\"\n    },\n    \"subtype\": {\n      \"type\": \"string\",\n      \"description\": \"Location sub-type (e.g. airport, port, rail-station, restaurant, atm...)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Label associated to the location (e.g. Eiffel Tower, Madison Square)\"\n    },\n    \"iataCode\": {\n      \"type\": \"string\",\n      \"description\": \"IATA location code\"\n    },\n    \"geoCode\": {\n      \"type\": \"object\",\n      \"description\": \"Geographic coordinates describing the position of any location on the surface of Earth\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\"\
  : \"number\",\n          \"description\": \"Latitude of the position expressed in decimal degrees (WSG 84), e.g. 6.244203. A positive value denotes northern hemisphere or the equator, and a negative value denotes southern hemisphere. The number of digits to represent the precision of the coordinate.\"\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"description\": \"Longitude of the position expressed in decimal degrees (WSG 84), e.g. -75.581211. A positive value denotes east longitude or the prime meridian, and a negative value denotes west longitude. The number of digits to represent the precision of the coordinate.\"\n        }\n      }\n    },\n    \"address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"countryName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the country of the location\"\n        },\n        \"countryCode\": {\n          \"type\": \"string\",\n          \"description\": \"Code\
  \ of the country of the location in ISO standard\"\n        },\n        \"stateCode\": {\n          \"type\": \"string\",\n          \"description\": \"Code of the state of the location (if any)\"\n        },\n        \"regionCode\": {\n          \"type\": \"string\",\n          \"description\": \"Code of the region of the location in ISO standard\"\n        }\n      }\n    },\n    \"timeZone\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"offSet\": {\n          \"type\": \"string\",\n          \"description\": \"'Total offset from UTC including the Daylight Saving Time (DST) following ISO 8601 (https://en.wikipedia.org/wiki/ISO_8601) standard'\"\n        },\n        \"referenceLocalDateTime\": {\n          \"type\": \"string\",\n          \"description\": \"Date and time used as reference to determine the time zone name, code, offset, and dstOffset following ISO 8601 (https://en.wikipedia.org/wiki/ISO_8601) standard.\"\n        }\n      }\n    },\n    \"metrics\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"relevance\": {\n          \"type\": \"integer\",\n          \"description\": \"Score value based on the number of travelers per year and per destination. Score is between 0 and 100, 100 being the value for the destination city with the highest value of travelers for the origin airport\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/airline-routes-locations-schema.json
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
title: locations
---
