---
description: Request body for searching future satellite capture opportunities.
layout: schema
name: TaskingSearchRequest
properties_list:
- description: Start of the search window.
  name: start
  type: string
- description: End of the search window.
  name: end
  type: string
- description: Maximum ground sample distance in meters.
  name: gsd
  type: number
- description: Latitude of the area of interest.
  name: lat
  type: number
- description: Longitude of the area of interest.
  name: long
  type: number
- description: Maximum acceptable cloud cover percentage.
  name: cloud
  type: integer
- description: Maximum off-nadir angle in degrees.
  name: offNadir
  type: number
- description: ''
  name: suppliers
  type: array
- description: ''
  name: platformTypes
  type: array
- description: ''
  name: sensorTypes
  type: array
provider_name: Arlula
provider_slug: arlula
schema_file: json-schema/arlula-tasking-search-request-schema.json
slug: arlula-tasking-search-request
source_filename: arlula-tasking-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://arlula.com/json-schema/tasking-search-request.json\",\n  \"title\": \"TaskingSearchRequest\",\n  \"description\": \"Request body for searching future satellite capture opportunities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"start\": {\n      \"type\": \"string\",\n      \"description\": \"Start of the search window.\",\n      \"examples\": [\n        \"2026-05-01T00:00:00Z\"\n      ]\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"description\": \"End of the search window.\",\n      \"examples\": [\n        \"2026-05-31T00:00:00Z\"\n      ]\n    },\n    \"gsd\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum ground sample distance in meters.\",\n      \"examples\": [\n        0.5\n      ]\n    },\n    \"lat\": {\n      \"type\": \"number\",\n      \"description\": \"Latitude of the area of interest.\",\n      \"examples\": [\n        -33.8523\n\
  \      ]\n    },\n    \"long\": {\n      \"type\": \"number\",\n      \"description\": \"Longitude of the area of interest.\",\n      \"examples\": [\n        151.2108\n      ]\n    },\n    \"cloud\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum acceptable cloud cover percentage.\",\n      \"examples\": [\n        20\n      ]\n    },\n    \"offNadir\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum off-nadir angle in degrees.\",\n      \"examples\": [\n        30.0\n      ]\n    },\n    \"suppliers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"platformTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sensorTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/arlula/refs/heads/main/json-schema/arlula-tasking-search-request-schema.json
tags:
- Earth Observation
- Geospatial
- Imagery
- Remote Sensing
- Satellites
title: TaskingSearchRequest
---
