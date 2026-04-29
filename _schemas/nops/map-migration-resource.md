---
description: A MAP Migration resource represents an individual AWS resource that is part of a MAP Migration project, tracked for migration and cost attribution.
layout: schema
name: nOps MAP Migration Resource
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
schema_file: json-schema/map-migration-resource.json
slug: map-migration-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nops/blob/main/json-schema/map-migration-resource.json\",\n  \"title\": \"nOps MAP Migration Resource\",\n  \"description\": \"A MAP Migration resource represents an individual AWS resource that is part of a MAP Migration project, tracked for migration and cost attribution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the resource.\"\n    },\n    \"resource_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the AWS resource.\"\n    },\n    \"resource_id\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS resource identifier.\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the parent MAP Migration project.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/json-schema/map-migration-resource.json
tags:
- Costs
- FinOps
title: nOps MAP Migration Resource
---
