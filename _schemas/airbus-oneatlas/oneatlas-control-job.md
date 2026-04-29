---
description: ''
layout: schema
name: ControlJob
properties_list:
- description: ''
  name: description
  type: string
- description: The control priority. The highest priority is 1.
  name: priority
  type: number
- description: The control steps to validate in order to complete control.
  name: steps
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-control-job-schema.json
slug: oneatlas-control-job
source_filename: oneatlas-control-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-control-job-schema.json\",\n  \"title\": \"ControlJob\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"description\": \"The control priority. The highest priority is 1.\",\n      \"example\": 1,\n      \"format\": \"integer\",\n      \"maximum\": 9,\n      \"minimum\": 1,\n      \"type\": \"number\"\n    },\n    \"steps\": {\n      \"description\": \"The control steps to validate in order to complete control.\",\n      \"items\": {\n        \"properties\": {\n          \"description\": {\n            \"description\": \"The control step definition.\",\n            \"type\": \"string\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"minItems\": 1,\n      \"type\": \"array\"\n    }\n\
  \  },\n  \"required\": [\n    \"description\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-control-job-schema.json
tags:
- Imagery
- Satellites
title: ControlJob
---
