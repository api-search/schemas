---
description: A movie in the Regal Entertainment Group cinema catalog
layout: schema
name: Movie
properties_list:
- description: Unique movie identifier
  name: id
  type: string
- description: Movie title
  name: title
  type: string
- description: Brief movie synopsis
  name: synopsis
  type: string
- description: MPAA content rating
  name: rating
  type: string
- description: Runtime in minutes
  name: runtime
  type: integer
- description: Theatrical release date (YYYY-MM-DD)
  name: releaseDate
  type: string
- description: List of genres
  name: genres
  type: array
- description: URL to movie poster image
  name: poster
  type: string
- description: URL to movie trailer
  name: trailerUrl
  type: string
- description: Principal cast members
  name: cast
  type: array
- description: Director name
  name: director
  type: string
- description: Current release status
  name: status
  type: string
provider_name: regal-entertainment-group
provider_slug: regal-entertainment-group
schema_file: json-schema/regal-movie-schema.json
slug: regal-movie
source_filename: regal-movie-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/regal-entertainment-group/json-schema/regal-movie-schema.json\",\n  \"title\": \"Movie\",\n  \"description\": \"A movie in the Regal Entertainment Group cinema catalog\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"title\", \"rating\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique movie identifier\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Movie title\"\n    },\n    \"synopsis\": {\n      \"type\": \"string\",\n      \"description\": \"Brief movie synopsis\"\n    },\n    \"rating\": {\n      \"type\": \"string\",\n      \"enum\": [\"G\", \"PG\", \"PG-13\", \"R\", \"NC-17\"],\n      \"description\": \"MPAA content rating\"\n    },\n    \"runtime\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Runtime in minutes\"\n\
  \    },\n    \"releaseDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Theatrical release date (YYYY-MM-DD)\"\n    },\n    \"genres\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"List of genres\"\n    },\n    \"poster\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to movie poster image\"\n    },\n    \"trailerUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to movie trailer\"\n    },\n    \"cast\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Principal cast members\"\n    },\n    \"director\": {\n      \"type\": \"string\",\n      \"description\": \"Director name\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"now_playing\", \"upcoming\"],\n      \"description\": \"Current release status\"\n    }\n  },\n  \"additionalProperties\"\
  : false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/regal-entertainment-group/refs/heads/main/json-schema/regal-movie-schema.json
tags:
- Cinema
- Entertainment
- Movies
- Ticketing
- Loyalty
- Theatre
- Fortune 500
title: Movie
---
