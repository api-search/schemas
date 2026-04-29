---
description: ''
layout: schema
name: geo-json-multipolygon
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
schema_file: json-schema/oneatlas-geo-json-multipolygon-schema.json
slug: oneatlas-geo-json-multipolygon
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-geo-json-multipolygon-schema.json\",\n  \"title\": \"geo-json-multipolygon\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MultiPolygon\"\n      ]\n    },\n    \"coordinates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"array\",\n          \"minItems\": 4,\n          \"items\": {\n            \"type\": \"array\",\n            \"minItems\": 2,\n            \"items\": {\n              \"type\": \"number\"\n            }\n          }\n        }\n      }\n    },\n    \"bbox\": {\n      \"type\": \"array\",\n      \"minItems\": 4,\n      \"items\": {\n        \"type\": \"number\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"\
  coordinates\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-geo-json-multipolygon-schema.json
tags:
- Imagery
- Satellites
title: geo-json-multipolygon
---
