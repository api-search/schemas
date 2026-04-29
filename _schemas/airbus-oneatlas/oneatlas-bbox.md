---
description: ''
layout: schema
name: bbox
properties_list:
- description: ''
  name: lr
  type: object
- description: ''
  name: srs
  type: object
- description: ''
  name: ul
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-bbox-schema.json
slug: oneatlas-bbox
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-bbox-schema.json\",\n  \"title\": \"bbox\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lr\": {\n      \"$ref\": \"#/components/schemas/point\"\n    },\n    \"srs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/srs\"\n        },\n        {\n          \"description\": \"Referential for the points of this bbox.\",\n          \"properties\": {\n            \"type\": {\n              \"enum\": [\n                \"urn\",\n                \"epsg\",\n                \"image\"\n              ]\n            }\n          },\n          \"type\": \"object\"\n        }\n      ]\n    },\n    \"ul\": {\n      \"$ref\": \"#/components/schemas/point\"\n    }\n  },\n  \"required\": [\n    \"srs\",\n    \"ul\",\n    \"lr\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-bbox-schema.json
tags:
- Imagery
- Satellites
title: bbox
---
