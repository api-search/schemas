---
description: Link object
layout: schema
name: Link
properties_list:
- description: The absolute web link
  name: href
  type: string
- description: HTTP verb to distinguish between several possible actions on the same ressource.
  name: method
  type: string
- description: The name of the link
  name: name
  type: string
- description: ''
  name: resourceId
  type: object
- description: The mime-type when deferencing the link
  name: type
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-link-schema.json
slug: oneatlas-link
source_filename: oneatlas-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-link-schema.json\",\n  \"title\": \"Link\",\n  \"type\": \"object\",\n  \"description\": \"Link object\",\n  \"properties\": {\n    \"href\": {\n      \"description\": \"The absolute web link\",\n      \"example\": \"https://monitoring.oneatlas.geoapi-airbusds.com/api/v1/activities/6b7a749b-64fb-48cd-ae68-39c0bbbe5051\",\n      \"format\": \"uri\",\n      \"type\": \"string\"\n    },\n    \"method\": {\n      \"default\": \"GET\",\n      \"description\": \"HTTP verb to distinguish between several possible actions on the same ressource.\",\n      \"enum\": [\n        \"GET\",\n        \"POST\",\n        \"PUT\",\n        \"DELETE\",\n        \"HEAD\"\n      ],\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the link\",\n      \"example\": \"Self\",\n \
  \     \"type\": \"string\"\n    },\n    \"resourceId\": {\n      \"$ref\": \"#/components/schemas/Id\"\n    },\n    \"type\": {\n      \"description\": \"The mime-type when deferencing the link\",\n      \"example\": \"application/json\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"href\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-link-schema.json
tags:
- Imagery
- Satellites
title: Link
---
