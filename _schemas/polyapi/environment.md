---
description: An environment for organizing and deploying resources across development, staging, and production in PolyAPI.
layout: schema
name: PolyAPI Environment
properties_list:
- description: The unique identifier of the environment.
  name: id
  type: string
- description: The name of the environment.
  name: name
  type: string
- description: A description of the environment.
  name: description
  type: string
- description: The context name attribute for the environment.
  name: contextName
  type: string
- description: Timestamp when the environment was created.
  name: createdAt
  type: string
- description: Timestamp when the environment was last updated.
  name: updatedAt
  type: string
provider_name: PolyAPI
provider_slug: polyapi
schema_file: json-schema/environment.json
slug: environment
source_filename: environment.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/polyapi/blob/main/json-schema/environment.json\",\n  \"title\": \"PolyAPI Environment\",\n  \"description\": \"An environment for organizing and deploying resources across development, staging, and production in PolyAPI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the environment.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the environment.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the environment.\"\n    },\n    \"contextName\": {\n      \"type\": \"string\",\n      \"description\": \"The context name attribute for the environment.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\":\
  \ \"Timestamp when the environment was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the environment was last updated.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/json-schema/environment.json
tags:
- Integrations
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
title: PolyAPI Environment
---
