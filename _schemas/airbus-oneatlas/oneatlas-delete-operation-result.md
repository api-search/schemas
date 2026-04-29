---
description: ''
layout: schema
name: DeleteOperationResult
properties_list:
- description: The number of deleted items
  name: deleted
  type: number
- description: The number of item deletion failures
  name: failures
  type: number
- description: The number of items not found
  name: notFound
  type: number
- description: The number of processed items
  name: total
  type: number
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-delete-operation-result-schema.json
slug: oneatlas-delete-operation-result
source_filename: oneatlas-delete-operation-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-delete-operation-result-schema.json\",\n  \"title\": \"DeleteOperationResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deleted\": {\n      \"description\": \"The number of deleted items\",\n      \"format\": \"integer\",\n      \"type\": \"number\"\n    },\n    \"failures\": {\n      \"description\": \"The number of item deletion failures\",\n      \"format\": \"integer\",\n      \"type\": \"number\"\n    },\n    \"notFound\": {\n      \"description\": \"The number of items not found\",\n      \"format\": \"integer\",\n      \"type\": \"number\"\n    },\n    \"total\": {\n      \"description\": \"The number of processed items\",\n      \"format\": \"integer\",\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-delete-operation-result-schema.json
tags:
- Imagery
- Satellites
title: DeleteOperationResult
---
