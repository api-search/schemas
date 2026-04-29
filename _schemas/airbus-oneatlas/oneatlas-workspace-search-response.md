---
description: ''
layout: schema
name: WorkspaceSearchResponse
properties_list:
- description: ''
  name: data
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-workspace-search-response-schema.json
slug: oneatlas-workspace-search-response
source_filename: oneatlas-workspace-search-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-workspace-search-response-schema.json\",\n  \"title\": \"WorkspaceSearchResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Workspace\"\n      },\n      \"type\": \"array\",\n      \"uniqueItems\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-workspace-search-response-schema.json
tags:
- Imagery
- Satellites
title: WorkspaceSearchResponse
---
