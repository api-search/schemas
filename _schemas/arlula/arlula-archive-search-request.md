---
description: Request body for searching the archive imagery catalog.
layout: schema
name: ArchiveSearchRequest
properties_list:
- description: Start date for imagery search (YYYY-MM-DD).
  name: start
  type: string
- description: End date for imagery search (YYYY-MM-DD).
  name: end
  type: string
- description: Maximum ground sample distance in meters.
  name: gsd
  type: number
- description: Latitude of the point of interest.
  name: lat
  type: number
- description: Longitude of the point of interest.
  name: long
  type: number
- description: Maximum cloud cover percentage (0-100).
  name: cloud
  type: integer
- description: Maximum off-nadir angle in degrees.
  name: offNadir
  type: number
- description: ''
  name: suppliers
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-archive-search-request-schema.json
slug: arlula-archive-search-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/archive-search-request.json\",\n  \"title\": \"ArchiveSearchRequest\",\n  \"description\": \"Request body for searching the archive imagery catalog.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"type\": \"string\",\n      \"description\": \"Start date for imagery search (YYYY-MM-DD).\",\n      \"examples\": [\n        \"2025-01-01\"\n      ]\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"description\": \"End date for imagery search (YYYY-MM-DD).\",\n      \"examples\": [\n        \"2025-03-31\"\n      ]\n    },\n    \"gsd\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum ground sample distance in meters.\",\n      \"examples\": [\n        1.5\n      ]\n    },\n    \"lat\": {\n      \"type\": \"number\",\n      \"description\": \"Latitude of the point of interest.\",\n      \"examples\": [\n        -33.8523\n\
  \      ]\n    },\n    \"long\": {\n      \"type\": \"number\",\n      \"description\": \"Longitude of the point of interest.\",\n      \"examples\": [\n        151.2108\n      ]\n    },\n    \"cloud\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum cloud cover percentage (0-100).\",\n      \"examples\": [\n        20\n      ]\n    },\n    \"offNadir\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum off-nadir angle in degrees.\",\n      \"examples\": [\n        30.0\n      ]\n    },\n    \"suppliers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-archive-search-request-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: ArchiveSearchRequest
---
