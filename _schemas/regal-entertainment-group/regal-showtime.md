---
description: A movie showtime at a Regal theatre
layout: schema
name: Showtime
properties_list:
- description: Unique showtime identifier
  name: id
  type: string
- description: Associated movie identifier
  name: movieId
  type: string
- description: Associated theatre identifier
  name: theatreId
  type: string
- description: Showtime start in ISO 8601 format
  name: startTime
  type: string
- description: Screening format
  name: format
  type: string
- description: Number of remaining available seats
  name: seatsAvailable
  type: integer
- description: ''
  name: price
  type: object
- description: Auditorium or screen identifier within the theatre
  name: auditorium
  type: string
provider_name: regal-entertainment-group
provider_slug: regal-entertainment-group
schema_file: json-schema/regal-showtime-schema.json
slug: regal-showtime
source_filename: regal-showtime-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/regal-entertainment-group/json-schema/regal-showtime-schema.json\",\n  \"title\": \"Showtime\",\n  \"description\": \"A movie showtime at a Regal theatre\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"movieId\", \"theatreId\", \"startTime\", \"format\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique showtime identifier\"\n    },\n    \"movieId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated movie identifier\"\n    },\n    \"theatreId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated theatre identifier\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Showtime start in ISO 8601 format\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\"IMAX\", \"4DX\", \"RPX\", \"\
  2D\", \"3D\"],\n      \"description\": \"Screening format\"\n    },\n    \"seatsAvailable\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of remaining available seats\"\n    },\n    \"price\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"adult\": { \"type\": \"number\", \"description\": \"Adult ticket price USD\" },\n        \"child\": { \"type\": \"number\", \"description\": \"Child ticket price USD\" },\n        \"senior\": { \"type\": \"number\", \"description\": \"Senior ticket price USD\" },\n        \"currency\": { \"type\": \"string\", \"default\": \"USD\" }\n      }\n    },\n    \"auditorium\": {\n      \"type\": \"string\",\n      \"description\": \"Auditorium or screen identifier within the theatre\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/regal-entertainment-group/refs/heads/main/json-schema/regal-showtime-schema.json
tags:
- Cinema
- Entertainment
- Movies
- Ticketing
- Loyalty
- Theatre
- Fortune 500
title: Showtime
---
