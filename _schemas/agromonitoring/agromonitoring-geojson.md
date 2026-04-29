---
description: GeoJSON polygon geometry defining a field boundary.
layout: schema
name: GeoJson
properties_list:
- description: GeoJSON geometry type.
  name: type
  type: string
- description: Array of coordinate rings defining the polygon.
  name: coordinates
  type: array
provider_name: Agromonitoring
provider_slug: agromonitoring
schema_file: json-schema/agromonitoring-geojson-schema.json
slug: agromonitoring-geojson
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.agromonitoring.com/schemas/GeoJson.json\",\n  \"title\": \"GeoJson\",\n  \"type\": \"object\",\n  \"description\": \"GeoJSON polygon geometry defining a field boundary.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"GeoJSON geometry type.\",\n      \"example\": \"Polygon\"\n    },\n    \"coordinates\": {\n      \"type\": \"array\",\n      \"description\": \"Array of coordinate rings defining the polygon.\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"number\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/json-schema/agromonitoring-geojson-schema.json
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
title: GeoJson
---
