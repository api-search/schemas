---
description: ''
layout: schema
name: ApiKeyPage
properties_list:
- description: API Keys
  name: items
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-api-key-page-schema.json
slug: oneatlas-api-key-page
source_filename: oneatlas-api-key-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-api-key-page-schema.json\",\n  \"title\": \"ApiKeyPage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"description\": \"API Keys\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ApiKey\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-api-key-page-schema.json
tags:
- Imagery
- Satellites
title: ApiKeyPage
---
