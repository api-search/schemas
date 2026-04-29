---
description: Historical NDVI data record for a specific acquisition date.
layout: schema
name: NdviRecord
properties_list:
- description: Acquisition date as Unix timestamp.
  name: dt
  type: integer
- description: Satellite source.
  name: source
  type: string
- description: Cloud coverage percentage.
  name: cl
  type: number
- description: ''
  name: stats
  type: object
provider_name: Agromonitoring
provider_slug: agromonitoring
schema_file: json-schema/agromonitoring-ndvirecord-schema.json
slug: agromonitoring-ndvirecord
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.agromonitoring.com/schemas/NdviRecord.json\",\n  \"title\": \"NdviRecord\",\n  \"type\": \"object\",\n  \"description\": \"Historical NDVI data record for a specific acquisition date.\",\n  \"properties\": {\n    \"dt\": {\n      \"type\": \"integer\",\n      \"description\": \"Acquisition date as Unix timestamp.\",\n      \"example\": 1709000000\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Satellite source.\",\n      \"example\": \"Sentinel-2\"\n    },\n    \"cl\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Cloud coverage percentage.\",\n      \"example\": 5.2\n    },\n    \"stats\": {\n      \"$ref\": \"#/components/schemas/VegetationStats\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agromonitoring/refs/heads/main/json-schema/agromonitoring-ndvirecord-schema.json
tags:
- Agriculture
- Satellite Imagery
- Vegetation Indices
- Weather
- Precision Agriculture
- Remote Sensing
title: NdviRecord
---
