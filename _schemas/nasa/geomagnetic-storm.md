---
description: A geomagnetic storm event from NASA's DONKI space weather database.
layout: schema
name: Geomagnetic Storm
properties_list:
- description: Unique identifier for the geomagnetic storm.
  name: gstID
  type: string
- description: Start time of the geomagnetic storm.
  name: startTime
  type: string
- description: Kp index observations for this storm.
  name: allKpIndex
  type: array
provider_name: NASA
provider_slug: nasa
schema_file: json-schema/geomagnetic-storm.json
slug: geomagnetic-storm
source_filename: geomagnetic-storm.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nasa/blob/main/json-schema/geomagnetic-storm.json\",\n  \"title\": \"Geomagnetic Storm\",\n  \"description\": \"A geomagnetic storm event from NASA's DONKI space weather database.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gstID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the geomagnetic storm.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of the geomagnetic storm.\"\n    },\n    \"allKpIndex\": {\n      \"type\": \"array\",\n      \"description\": \"Kp index observations for this storm.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"observedTime\": { \"type\": \"string\", \"format\": \"date-time\" },\n          \"kpIndex\": { \"type\": \"number\" },\n          \"source\": { \"type\"\
  : \"string\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"gstID\", \"startTime\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/json-schema/geomagnetic-storm.json
tags:
- Government
- Science
- Space
title: Geomagnetic Storm
---
