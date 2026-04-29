---
description: Satellite imagery metadata with vegetation index statistics.
layout: schema
name: SatelliteImage
properties_list:
- description: Acquisition date as Unix timestamp.
  name: dt
  type: integer
- description: Satellite source (Sentinel-2 or Landsat-8).
  name: source
  type: string
- description: Cloud coverage percentage for this image.
  name: cl
  type: number
- description: Vegetation index statistics for the polygon.
  name: stats
  type: object
- description: URLs to image tiles (truecolor, falsecolor, ndvi).
  name: image
  type: object
provider_name: Agromonitoring
provider_slug: agromonitoring
schema_file: json-schema/agromonitoring-satelliteimage-schema.json
slug: agromonitoring-satelliteimage
source_filename: agromonitoring-satelliteimage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.agromonitoring.com/schemas/SatelliteImage.json\",\n  \"title\": \"SatelliteImage\",\n  \"type\": \"object\",\n  \"description\": \"Satellite imagery metadata with vegetation index statistics.\",\n  \"properties\": {\n    \"dt\": {\n      \"type\": \"integer\",\n      \"description\": \"Acquisition date as Unix timestamp.\",\n      \"example\": 1709000000\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Satellite source (Sentinel-2 or Landsat-8).\",\n      \"enum\": [\n        \"Sentinel-2\",\n        \"Landsat-8\"\n      ],\n      \"example\": \"Sentinel-2\"\n    },\n    \"cl\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Cloud coverage percentage for this image.\",\n      \"example\": 5.2\n    },\n    \"stats\": {\n      \"type\": \"object\",\n      \"description\": \"Vegetation index statistics for the polygon.\"\
  ,\n      \"properties\": {\n        \"ndvi\": {\n          \"$ref\": \"#/components/schemas/VegetationStats\"\n        }\n      }\n    },\n    \"image\": {\n      \"type\": \"object\",\n      \"description\": \"URLs to image tiles (truecolor, falsecolor, ndvi).\",\n      \"properties\": {\n        \"truecolor\": {\n          \"type\": \"string\",\n          \"description\": \"URL to the true color image tile.\",\n          \"example\": \"https://api.agromonitoring.com/agro/1.0/image/1/truecolor\"\n        },\n        \"falsecolor\": {\n          \"type\": \"string\",\n          \"description\": \"URL to the false color image tile.\",\n          \"example\": \"https://api.agromonitoring.com/agro/1.0/image/1/falsecolor\"\n        },\n        \"ndvi\": {\n          \"type\": \"string\",\n          \"description\": \"URL to the NDVI image tile.\",\n          \"example\": \"https://api.agromonitoring.com/agro/1.0/image/1/ndvi\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/json-schema/agromonitoring-satelliteimage-schema.json
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
title: SatelliteImage
---
