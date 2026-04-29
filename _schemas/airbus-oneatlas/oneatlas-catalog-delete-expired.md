---
description: ''
layout: schema
name: catalog-delete-expired
properties_list:
- description: List of workspaces where expired catalog items should be deleted. If not set, expired items of every worskapces will be deleted.
  name: workspaces
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-catalog-delete-expired-schema.json
slug: oneatlas-catalog-delete-expired
source_filename: oneatlas-catalog-delete-expired-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-catalog-delete-expired-schema.json\",\n  \"title\": \"catalog-delete-expired\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workspaces\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/WorkspaceIdentifier\"\n      },\n      \"description\": \"List of workspaces where expired catalog items should be deleted. If not set, expired items of every worskapces will be deleted.\",\n      \"minItems\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-catalog-delete-expired-schema.json
tags:
- Imagery
- Satellites
title: catalog-delete-expired
---
