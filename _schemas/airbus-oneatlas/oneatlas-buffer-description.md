---
description: ''
layout: schema
name: bufferDescription
properties_list:
- description: Ordered list of requested bands. Bands can be retrieve with `metadata` link given in `_links` property of a feature.
  name: bands
  type: array
- description: ''
  name: bbox
  type: object
- description: ''
  name: step
  type: object
- description: specification of the output buffer
  name: target-model
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-buffer-description-schema.json
slug: oneatlas-buffer-description
source_filename: oneatlas-buffer-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-buffer-description-schema.json\",\n  \"title\": \"bufferDescription\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bands\": {\n      \"default\": \"all bands\",\n      \"description\": \"Ordered list of requested bands. Bands can be retrieve with `metadata` link given in `_links` property of a feature.\",\n      \"items\": {\n        \"example\": \"R\",\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"bbox\": {\n      \"$ref\": \"#/components/schemas/bbox\"\n    },\n    \"step\": {\n      \"$ref\": \"#/components/schemas/step\"\n    },\n    \"target-model\": {\n      \"description\": \"specification of the output buffer\",\n      \"properties\": {\n        \"crs\": {\n          \"default\": \"Bbox srs\",\n          \"description\": \"Output crs.\",\n \
  \         \"example\": \"epsg:4326\",\n          \"type\": \"string\"\n        },\n        \"size\": {\n          \"$ref\": \"#/components/schemas/imageSize\"\n        }\n      },\n      \"type\": \"object\"\n    }\n  },\n  \"required\": [\n    \"bbox\",\n    \"step\",\n    \"target-model\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-buffer-description-schema.json
tags:
- Imagery
- Satellites
title: bufferDescription
---
