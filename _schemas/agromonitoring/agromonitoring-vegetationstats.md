---
description: Zonal statistics for a vegetation index over a polygon.
layout: schema
name: VegetationStats
properties_list:
- description: Minimum index value in the polygon.
  name: min
  type: number
- description: Maximum index value in the polygon.
  name: max
  type: number
- description: Mean index value.
  name: mean
  type: number
- description: Median index value.
  name: median
  type: number
- description: Standard deviation of index values.
  name: std
  type: number
provider_name: Agromonitoring
provider_slug: agromonitoring
schema_file: json-schema/agromonitoring-vegetationstats-schema.json
slug: agromonitoring-vegetationstats
source_filename: agromonitoring-vegetationstats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.agromonitoring.com/schemas/VegetationStats.json\",\n  \"title\": \"VegetationStats\",\n  \"type\": \"object\",\n  \"description\": \"Zonal statistics for a vegetation index over a polygon.\",\n  \"properties\": {\n    \"min\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Minimum index value in the polygon.\",\n      \"example\": 0.1\n    },\n    \"max\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Maximum index value in the polygon.\",\n      \"example\": 0.85\n    },\n    \"mean\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Mean index value.\",\n      \"example\": 0.62\n    },\n    \"median\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Median index value.\",\n      \"example\": 0.65\n    },\n    \"std\": {\n\
  \      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Standard deviation of index values.\",\n      \"example\": 0.12\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/json-schema/agromonitoring-vegetationstats-schema.json
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
title: VegetationStats
---
