---
description: ''
layout: schema
name: WorkspaceSearchOptions
properties_list:
- description: The name of the workspace
  name: name
  type: string
- description: ''
  name: userId
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-workspace-search-options-schema.json
slug: oneatlas-workspace-search-options
source_filename: oneatlas-workspace-search-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-workspace-search-options-schema.json\",\n  \"title\": \"WorkspaceSearchOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"The name of the workspace\",\n      \"example\": \"workspace de Jean-Charles\",\n      \"type\": \"string\"\n    },\n    \"userId\": {\n      \"$ref\": \"#/components/schemas/Id\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-workspace-search-options-schema.json
tags:
- Imagery
- Satellites
title: WorkspaceSearchOptions
---
