---
description: Weather conditions for a specific date and location.
layout: schema
name: WeatherData
properties_list:
- description: Date as Unix timestamp.
  name: dt
  type: integer
- description: ''
  name: temp
  type: object
- description: Relative humidity percentage.
  name: humidity
  type: integer
- description: Wind speed in m/s (or mph for imperial).
  name: wind_speed
  type: number
- description: Wind direction in degrees.
  name: wind_deg
  type: integer
- description: Cloud coverage percentage.
  name: clouds
  type: integer
- description: Precipitation amount in mm.
  name: rain
  type: number
- description: UV index value.
  name: uvi
  type: number
provider_name: Agromonitoring
provider_slug: agromonitoring
schema_file: json-schema/agromonitoring-weatherdata-schema.json
slug: agromonitoring-weatherdata
source_filename: agromonitoring-weatherdata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.agromonitoring.com/schemas/WeatherData.json\",\n  \"title\": \"WeatherData\",\n  \"type\": \"object\",\n  \"description\": \"Weather conditions for a specific date and location.\",\n  \"properties\": {\n    \"dt\": {\n      \"type\": \"integer\",\n      \"description\": \"Date as Unix timestamp.\",\n      \"example\": 1712000000\n    },\n    \"temp\": {\n      \"$ref\": \"#/components/schemas/TemperatureRange\"\n    },\n    \"humidity\": {\n      \"type\": \"integer\",\n      \"description\": \"Relative humidity percentage.\",\n      \"example\": 65\n    },\n    \"wind_speed\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Wind speed in m/s (or mph for imperial).\",\n      \"example\": 4.2\n    },\n    \"wind_deg\": {\n      \"type\": \"integer\",\n      \"description\": \"Wind direction in degrees.\",\n      \"example\": 180\n    },\n    \"\
  clouds\": {\n      \"type\": \"integer\",\n      \"description\": \"Cloud coverage percentage.\",\n      \"example\": 30\n    },\n    \"rain\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Precipitation amount in mm.\",\n      \"example\": 0.0\n    },\n    \"uvi\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"UV index value.\",\n      \"example\": 5.2\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/json-schema/agromonitoring-weatherdata-schema.json
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
title: WeatherData
---
