---
description: A MAP Migration product represents an AWS product or service within a MAP Migration project that is part of the migration effort.
layout: schema
name: nOps MAP Migration Product
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
schema_file: json-schema/map-migration-product.json
slug: map-migration-product
source_filename: map-migration-product.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nops/blob/main/json-schema/map-migration-product.json\",\n  \"title\": \"nOps MAP Migration Product\",\n  \"description\": \"A MAP Migration product represents an AWS product or service within a MAP Migration project that is part of the migration effort.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the product.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the product.\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the parent MAP Migration project.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/json-schema/map-migration-product.json
tags:
- Costs
- FinOps
title: nOps MAP Migration Product
---
