---
description: Daily temperature range data.
layout: schema
name: TemperatureRange
properties_list:
- description: Daytime temperature.
  name: day
  type: number
- description: Minimum temperature of the day.
  name: min
  type: number
- description: Maximum temperature of the day.
  name: max
  type: number
provider_name: Agromonitoring
provider_slug: agromonitoring
schema_file: json-schema/agromonitoring-temperaturerange-schema.json
slug: agromonitoring-temperaturerange
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.agromonitoring.com/schemas/TemperatureRange.json\",\n  \"title\": \"TemperatureRange\",\n  \"type\": \"object\",\n  \"description\": \"Daily temperature range data.\",\n  \"properties\": {\n    \"day\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Daytime temperature.\",\n      \"example\": 22.5\n    },\n    \"min\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Minimum temperature of the day.\",\n      \"example\": 15.3\n    },\n    \"max\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Maximum temperature of the day.\",\n      \"example\": 27.8\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/json-schema/agromonitoring-temperaturerange-schema.json
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
title: TemperatureRange
---
