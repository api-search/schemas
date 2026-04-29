---
description: Similar Location
layout: schema
name: RecommendedLocation
properties_list: []
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
schema_file: json-schema/travel-recommendations-recommended-location-schema.json
slug: travel-recommendations-recommended-location
source_filename: travel-recommendations-recommended-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/travel-recommendations-recommended-location-schema.json\",\n  \"title\": \"RecommendedLocation\",\n  \"description\": \"Similar Location\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"description\": \"Description of a particular point or place in physical space\",\n      \"title\": \"Location\",\n      \"properties\": {\n        \"subtype\": {\n          \"type\": \"string\",\n          \"description\": \"Location sub-type (e.g. airport, port, rail-station, restaurant, atm...)\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Label associated to the location (e.g. Eiffel Tower, Madison Square)\",\n          \"example\": \"Eiffel Tower\"\n        },\n        \"iataCode\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"IATA location code\",\n          \"example\": \"PAR\"\n        },\n        \"geoCode\": {\n          \"type\": \"object\",\n          \"description\": \"Geographic coordinates describing the position of any location on the surface of Earth\",\n          \"title\": \"GeoCode\",\n          \"properties\": {\n            \"latitude\": {\n              \"type\": \"number\",\n              \"format\": \"float\",\n              \"description\": \"Latitude of the position expressed in decimal degrees (WSG 84), e.g. 6.244203. A positive value denotes northern hemisphere or the equator, and a negative value denotes southern hemisphere. The number of digits to represent the precision of the coordinate.\",\n              \"minimum\": -90,\n              \"exclusiveMinimum\": false,\n              \"maximum\": 90,\n              \"exclusiveMaximum\": false,\n              \"example\": 48.85837\n            },\n            \"longitude\": {\n              \"type\": \"number\",\n              \"\
  format\": \"float\",\n              \"description\": \"Longitude of the position expressed in decimal degrees (WSG 84), e.g. -75.581211. A positive value denotes east longitude or the prime meridian, and a negative value denotes west longitude.  The number of digits to represent the precision of the coordinate.\",\n              \"minimum\": -180,\n              \"exclusiveMinimum\": false,\n              \"maximum\": 180,\n              \"exclusiveMaximum\": false,\n              \"example\": 2.294481\n            }\n          }\n        }\n      }\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Ressource type\"\n        },\n        \"relevance\": {\n          \"type\": \"number\",\n          \"description\": \"percentage of similarity.\\n\\n0 for not similar to 1 for exactly the same\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/json-schema/travel-recommendations-recommended-location-schema.json
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
title: RecommendedLocation
---
