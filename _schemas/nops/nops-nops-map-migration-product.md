---
description: ''
layout: schema
name: MapMigrationProduct
properties_list:
- description: The unique identifier of the product.
  name: id
  type: integer
- description: The name of the product.
  name: name
  type: string
- description: The ID of the parent MAP Migration project.
  name: project_id
  type: integer
provider_name: nOps
provider_slug: nops
schema_file: json-schema/nops-nops-map-migration-product-schema.json
slug: nops-nops-map-migration-product
source_filename: nops-nops-map-migration-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MapMigrationProduct\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the product.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the product.\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the parent MAP Migration project.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/json-schema/nops-nops-map-migration-product-schema.json
tags:
- Costs
- FinOps
title: MapMigrationProduct
---
