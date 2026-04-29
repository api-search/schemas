---
description: A geo point.
layout: schema
name: point
properties_list:
- description: x coordinate
  name: x
  type: number
- description: y coordinate
  name: y
  type: number
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-point-schema.json
slug: oneatlas-point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-point-schema.json\",\n  \"title\": \"point\",\n  \"type\": \"object\",\n  \"description\": \"A geo point.\",\n  \"properties\": {\n    \"x\": {\n      \"description\": \"x coordinate\",\n      \"type\": \"number\"\n    },\n    \"y\": {\n      \"description\": \"y coordinate\",\n      \"type\": \"number\"\n    }\n  },\n  \"required\": [\n    \"x\",\n    \"y\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-point-schema.json
tags:
- Imagery
- Satellites
title: point
---
