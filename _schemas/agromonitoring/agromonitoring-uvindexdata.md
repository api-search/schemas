---
description: UV radiation index for a location.
layout: schema
name: UvIndexData
properties_list:
- description: Latitude of the location.
  name: lat
  type: number
- description: Longitude of the location.
  name: lon
  type: number
- description: Measurement date in ISO 8601 format.
  name: date_iso
  type: string
- description: Measurement date as Unix timestamp.
  name: date
  type: integer
- description: UV index value (scale 0-11+).
  name: value
  type: number
provider_name: Agromonitoring
provider_slug: agromonitoring
schema_file: json-schema/agromonitoring-uvindexdata-schema.json
slug: agromonitoring-uvindexdata
source_filename: agromonitoring-uvindexdata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.agromonitoring.com/schemas/UvIndexData.json\",\n  \"title\": \"UvIndexData\",\n  \"type\": \"object\",\n  \"description\": \"UV radiation index for a location.\",\n  \"properties\": {\n    \"lat\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Latitude of the location.\",\n      \"example\": 38.5\n    },\n    \"lon\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Longitude of the location.\",\n      \"example\": -94.5\n    },\n    \"date_iso\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Measurement date in ISO 8601 format.\",\n      \"example\": \"2026-04-19T12:00:00Z\"\n    },\n    \"date\": {\n      \"type\": \"integer\",\n      \"description\": \"Measurement date as Unix timestamp.\",\n      \"example\": 1712000000\n    },\n    \"value\": {\n      \"\
  type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"UV index value (scale 0-11+).\",\n      \"example\": 5.2\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/json-schema/agromonitoring-uvindexdata-schema.json
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
title: UvIndexData
---
