---
description: ''
layout: schema
name: footprint
properties_list:
- description: ''
  name: geometry
  type: string
- description: ''
  name: center
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-footprint-schema.json
slug: oneatlas-footprint
source_filename: oneatlas-footprint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-footprint-schema.json\",\n  \"title\": \"footprint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"geometry\": {\n      \"type\": \"string\",\n      \"example\": \"POLYGON((23.642028 38.043069, 23.642495 37.909283, 23.868104 37.908839, 23.868548 38.04307, 23.642028 38.043069, 23.642028 38.043069))\"\n    },\n    \"center\": {\n      \"type\": \"string\",\n      \"example\": \"POINT(23.755357 37.97611)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-footprint-schema.json
tags:
- Imagery
- Satellites
title: footprint
---
