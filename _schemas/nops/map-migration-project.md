---
description: A MAP Migration project represents an AWS Migration Acceleration Program engagement signed by the customer with AWS, tracking the overall migration effort.
layout: schema
name: nOps MAP Migration Project
properties_list:
- description: The unique identifier of the MAP Migration project.
  name: id
  type: integer
- description: The name of the MAP Migration project.
  name: name
  type: string
- description: The current status of the project.
  name: status
  type: string
- description: Timestamp when the project was created.
  name: created_at
  type: string
- description: Timestamp when the project was last updated.
  name: updated_at
  type: string
provider_name: nOps
provider_slug: nops
schema_file: json-schema/map-migration-project.json
slug: map-migration-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nops/blob/main/json-schema/map-migration-project.json\",\n  \"title\": \"nOps MAP Migration Project\",\n  \"description\": \"A MAP Migration project represents an AWS Migration Acceleration Program engagement signed by the customer with AWS, tracking the overall migration effort.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the MAP Migration project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the MAP Migration project.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the project.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project was created.\"\n    },\n    \"\
  updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/json-schema/map-migration-project.json
tags:
- Costs
- FinOps
title: nOps MAP Migration Project
---
