---
description: Referential
layout: schema
name: srs
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: value
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-srs-schema.json
slug: oneatlas-srs
source_filename: oneatlas-srs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-srs-schema.json\",\n  \"title\": \"srs\",\n  \"type\": \"object\",\n  \"description\": \"Referential\",\n  \"properties\": {\n    \"type\": {\n      \"enum\": [\n        \"urn\",\n        \"epsg\",\n        \"proj4\"\n      ],\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"example\": \"urn:ogc:def:crs:EPSG::4326\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-srs-schema.json
tags:
- Imagery
- Satellites
title: srs
---
