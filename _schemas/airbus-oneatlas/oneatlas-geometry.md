---
description: ''
layout: schema
name: geometry
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: coordinates
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-geometry-schema.json
slug: oneatlas-geometry
source_filename: oneatlas-geometry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-geometry-schema.json\",\n  \"title\": \"geometry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"enum\": [\n        \"Polygon\"\n      ],\n      \"type\": \"string\"\n    },\n    \"coordinates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"format\": \"float\",\n            \"type\": \"number\"\n          },\n          \"maxItems\": 2\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-geometry-schema.json
tags:
- Imagery
- Satellites
title: geometry
---
