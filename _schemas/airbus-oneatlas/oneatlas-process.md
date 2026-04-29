---
description: a JSON Object that conforms to the InfoObject as specified in the Describe Process Specification v1.0
layout: schema
name: process
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: family
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: label
  type: string
- description: ''
  name: version
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-process-schema.json
slug: oneatlas-process
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-process-schema.json\",\n  \"title\": \"process\",\n  \"type\": \"object\",\n  \"description\": \"a JSON Object that conforms to the InfoObject as specified in the Describe Process Specification v1.0\",\n  \"properties\": {\n    \"description\": {\n      \"example\": \"process ortho rectification of a pack\",\n      \"type\": \"string\"\n    },\n    \"family\": {\n      \"example\": \"Ortho\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"example\": \"com.airbus.massive.ortho\",\n      \"type\": \"string\"\n    },\n    \"label\": {\n      \"example\": \"MassiveOrtho\",\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"example\": 1,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-process-schema.json
tags:
- Imagery
- Satellites
title: process
---
