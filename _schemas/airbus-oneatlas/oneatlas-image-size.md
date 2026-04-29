---
description: size (in pixels) of the result
layout: schema
name: imageSize
properties_list:
- description: number of columns of the output buffer
  name: columns
  type: number
- description: number of lines of the output buffer
  name: lines
  type: number
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-image-size-schema.json
slug: oneatlas-image-size
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-image-size-schema.json\",\n  \"title\": \"imageSize\",\n  \"type\": \"object\",\n  \"description\": \"size (in pixels) of the result\",\n  \"properties\": {\n    \"columns\": {\n      \"description\": \"number of columns of the output buffer\",\n      \"example\": 500,\n      \"format\": \"integer\",\n      \"maximum\": 5000,\n      \"minimum\": 1,\n      \"type\": \"number\"\n    },\n    \"lines\": {\n      \"description\": \"number of lines of the output buffer\",\n      \"example\": 500,\n      \"format\": \"integer\",\n      \"maximum\": 5000,\n      \"minimum\": 1,\n      \"type\": \"number\"\n    }\n  },\n  \"required\": [\n    \"columns\",\n    \"lines\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-image-size-schema.json
tags:
- Imagery
- Satellites
title: imageSize
---
