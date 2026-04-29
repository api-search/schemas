---
description: Meta information about the returned object(s) in "data"
layout: schema
name: Meta
properties_list:
- description: Total number of object(s) retrieved
  name: count
  type: integer
- description: Sorting fields criteria and their associated priority and direction. Sorting priority is indicated by the order of the strings within the array. E.g. sort=title,size means that items are ordered by ti
  name: sort
  type: array
- description: Links related to the returned object(s)
  name: links
  type: object
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/hotel-list-meta-schema.json
slug: hotel-list-meta
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Meta\",\n  \"description\": \"Meta information about the returned object(s) in \\\"data\\\"\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total number of object(s) retrieved\"\n    },\n    \"sort\": {\n      \"type\": \"array\",\n      \"description\": \"Sorting fields criteria and their associated priority and direction. Sorting priority is indicated by the order of the strings within the array. E.g. sort=title,size means that items are ordered by title and then, as a second ordering by size. A '-' sign before the search criteria indicates a descending ordering direction (Z to A), whereas no sign indicates a ascending direction (A to Z). E.g. sort=-title mean that the objects are ordered by title in reverse order (Z to A).\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n\
  \    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Links related to the returned object(s)\",\n      \"properties\": {\n        \"self\": {\n          \"type\": \"string\",\n          \"format\": \"url\",\n          \"description\": \"Link to the same page.\"\n        },\n        \"first\": {\n          \"type\": \"string\",\n          \"format\": \"url\",\n          \"description\": \"Link to the first page.\"\n        },\n        \"prev\": {\n          \"type\": \"string\",\n          \"format\": \"url\",\n          \"description\": \"Link to the previous page.\"\n        },\n        \"next\": {\n          \"type\": \"string\",\n          \"format\": \"url\",\n          \"description\": \"Link to the next page.\"\n        },\n        \"last\": {\n          \"type\": \"string\",\n          \"format\": \"url\",\n          \"description\": \"Link to the last page.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/hotel-list-meta-schema.json
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
title: Meta
---
