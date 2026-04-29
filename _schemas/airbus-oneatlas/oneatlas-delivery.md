---
description: ''
layout: schema
name: delivery
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: workspace
  type: object
- description: ''
  name: platformId
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-delivery-schema.json
slug: oneatlas-delivery
source_filename: oneatlas-delivery-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-delivery-schema.json\",\n  \"title\": \"delivery\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"network\"\n      ]\n    },\n    \"workspace\": {\n      \"$ref\": \"#/components/schemas/workspace\"\n    },\n    \"platformId\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PublicMOC\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-delivery-schema.json
tags:
- Imagery
- Satellites
title: delivery
---
