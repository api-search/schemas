---
description: ''
layout: schema
name: MapMigrationResource
properties_list:
- description: The unique identifier of the resource.
  name: id
  type: integer
- description: The type of the AWS resource.
  name: resource_type
  type: string
- description: The AWS resource identifier.
  name: resource_id
  type: string
- description: The ID of the parent MAP Migration project.
  name: project_id
  type: integer
provider_name: nOps
provider_slug: nops
schema_file: json-schema/nops-nops-map-migration-resource-schema.json
slug: nops-nops-map-migration-resource
source_filename: nops-nops-map-migration-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MapMigrationResource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the resource.\"\n    },\n    \"resource_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the AWS resource.\"\n    },\n    \"resource_id\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS resource identifier.\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the parent MAP Migration project.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/json-schema/nops-nops-map-migration-resource-schema.json
tags:
- Costs
- FinOps
title: MapMigrationResource
---
