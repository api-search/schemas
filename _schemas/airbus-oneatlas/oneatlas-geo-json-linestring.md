---
description: ''
layout: schema
name: geo-json-linestring
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: coordinates
  type: array
- description: ''
  name: bbox
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-geo-json-linestring-schema.json
slug: oneatlas-geo-json-linestring
source_filename: oneatlas-geo-json-linestring-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-geo-json-linestring-schema.json\",\n  \"title\": \"geo-json-linestring\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LineString\"\n      ]\n    },\n    \"coordinates\": {\n      \"type\": \"array\",\n      \"minItems\": 2,\n      \"items\": {\n        \"type\": \"array\",\n        \"minItems\": 2,\n        \"items\": {\n          \"type\": \"number\"\n        }\n      }\n    },\n    \"bbox\": {\n      \"type\": \"array\",\n      \"minItems\": 4,\n      \"items\": {\n        \"type\": \"number\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"coordinates\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-geo-json-linestring-schema.json
tags:
- Imagery
- Satellites
title: geo-json-linestring
---
