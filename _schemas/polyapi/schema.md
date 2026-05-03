---
description: A shared JSON Schema definition used to type events and application data across PolyAPI functions and webhooks.
layout: schema
name: PolyAPI Schema
properties_list:
- description: The unique identifier of the schema.
  name: id
  type: string
- description: The name of the schema.
  name: name
  type: string
- description: A description of the schema.
  name: description
  type: string
- description: The context path for organizing the schema in the catalog.
  name: context
  type: string
- description: The JSON Schema definition.
  name: definition
  type: object
- description: The visibility of the schema.
  name: visibility
  type: string
- description: Timestamp when the schema was created.
  name: createdAt
  type: string
- description: Timestamp when the schema was last updated.
  name: updatedAt
  type: string
provider_name: PolyAPI
provider_slug: polyapi
schema_file: json-schema/schema.json
slug: schema
source_filename: schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/polyapi/blob/main/json-schema/schema.json\",\n  \"title\": \"PolyAPI Schema\",\n  \"description\": \"A shared JSON Schema definition used to type events and application data across PolyAPI functions and webhooks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the schema.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the schema.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the schema.\"\n    },\n    \"context\": {\n      \"type\": \"string\",\n      \"description\": \"The context path for organizing the schema in the catalog.\"\n    },\n    \"definition\": {\n      \"type\": \"object\",\n      \"description\": \"The JSON Schema definition.\"\n    },\n    \"visibility\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\"],\n      \"description\": \"The visibility of the schema.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the schema was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the schema was last updated.\"\n    }\n  },\n  \"required\": [\"name\", \"definition\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/json-schema/schema.json
tags:
- Integrations
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
title: PolyAPI Schema
---
