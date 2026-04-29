---
description: Soil temperature and moisture data for a polygon.
layout: schema
name: SoilData
properties_list:
- description: Measurement date as Unix timestamp.
  name: dt
  type: integer
- description: Soil surface temperature in Celsius.
  name: t0
  type: number
- description: Soil temperature at 10cm depth in Celsius.
  name: t10
  type: number
- description: Volumetric soil moisture (0 to 1 scale).
  name: moisture
  type: number
provider_name: Agromonitoring
provider_slug: agromonitoring
schema_file: json-schema/agromonitoring-soildata-schema.json
slug: agromonitoring-soildata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.agromonitoring.com/schemas/SoilData.json\",\n  \"title\": \"SoilData\",\n  \"type\": \"object\",\n  \"description\": \"Soil temperature and moisture data for a polygon.\",\n  \"properties\": {\n    \"dt\": {\n      \"type\": \"integer\",\n      \"description\": \"Measurement date as Unix timestamp.\",\n      \"example\": 1712000000\n    },\n    \"t0\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Soil surface temperature in Celsius.\",\n      \"example\": 18.5\n    },\n    \"t10\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Soil temperature at 10cm depth in Celsius.\",\n      \"example\": 15.2\n    },\n    \"moisture\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Volumetric soil moisture (0 to 1 scale).\",\n      \"example\": 0.42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/json-schema/agromonitoring-soildata-schema.json
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
title: SoilData
---
