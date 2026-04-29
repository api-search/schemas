---
description: Resolution (step) of the image in the output referential. Unit must respect the srs definition.
layout: schema
name: step
properties_list:
- description: Unit of the step
  name: unit
  type: string
- description: ''
  name: x
  type: number
- description: ''
  name: y
  type: number
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-step-schema.json
slug: oneatlas-step
source_filename: oneatlas-step-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-step-schema.json\",\n  \"title\": \"step\",\n  \"type\": \"object\",\n  \"description\": \"Resolution (step) of the image in the output referential. Unit must respect the srs definition.\",\n  \"properties\": {\n    \"unit\": {\n      \"description\": \"Unit of the step\",\n      \"enum\": [\n        \"degree\"\n      ],\n      \"type\": \"string\"\n    },\n    \"x\": {\n      \"type\": \"number\"\n    },\n    \"y\": {\n      \"type\": \"number\"\n    }\n  },\n  \"required\": [\n    \"x\",\n    \"y\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-step-schema.json
tags:
- Imagery
- Satellites
title: step
---
