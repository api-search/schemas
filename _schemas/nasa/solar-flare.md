---
description: A solar flare event from NASA's DONKI space weather database.
layout: schema
name: Solar Flare
properties_list:
- description: Unique identifier for the solar flare event.
  name: flrID
  type: string
- description: ''
  name: instruments
  type: array
- description: Start time of the solar flare.
  name: beginTime
  type: string
- description: Peak time of the solar flare.
  name: peakTime
  type: string
- description: End time of the solar flare.
  name: endTime
  type: string
- description: Classification of the flare (e.g. X, M, C, B, A).
  name: classType
  type: string
- description: Location on the Sun where the flare originated.
  name: sourceLocation
  type: string
- description: Active region number on the Sun.
  name: activeRegionNum
  type: integer
provider_name: NASA
provider_slug: nasa
schema_file: json-schema/solar-flare.json
slug: solar-flare
source_filename: solar-flare.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nasa/blob/main/json-schema/solar-flare.json\",\n  \"title\": \"Solar Flare\",\n  \"description\": \"A solar flare event from NASA's DONKI space weather database.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flrID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the solar flare event.\"\n    },\n    \"instruments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"displayName\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"beginTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of the solar flare.\"\n    },\n    \"peakTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Peak time of the solar flare.\"\n    },\n    \"endTime\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"End time of the solar flare.\"\n    },\n    \"classType\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the flare (e.g. X, M, C, B, A).\"\n    },\n    \"sourceLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Location on the Sun where the flare originated.\"\n    },\n    \"activeRegionNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Active region number on the Sun.\"\n    }\n  },\n  \"required\": [\"flrID\", \"beginTime\", \"classType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/json-schema/solar-flare.json
tags:
- Government
- Science
- Space
title: Solar Flare
---
