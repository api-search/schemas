---
description: A client function is a shared function that runs wherever it is executed, rather than in the PolyAPI cloud infrastructure.
layout: schema
name: PolyAPI Client Function
properties_list:
- description: The unique identifier of the client function.
  name: id
  type: string
- description: The name of the client function.
  name: name
  type: string
- description: A description of what the client function does.
  name: description
  type: string
- description: The context path for organizing the function in the catalog.
  name: context
  type: string
- description: The programming language of the function.
  name: language
  type: string
- description: The function source code.
  name: code
  type: string
- description: The lifecycle state of the function.
  name: state
  type: string
- description: The owner of the function.
  name: owner
  type: string
- description: The visibility of the function.
  name: visibility
  type: string
- description: Timestamp when the function was created.
  name: createdAt
  type: string
- description: Timestamp when the function was last updated.
  name: updatedAt
  type: string
provider_name: PolyAPI
provider_slug: polyapi
schema_file: json-schema/client-function.json
slug: client-function
source_filename: client-function.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/polyapi/blob/main/json-schema/client-function.json\",\n  \"title\": \"PolyAPI Client Function\",\n  \"description\": \"A client function is a shared function that runs wherever it is executed, rather than in the PolyAPI cloud infrastructure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the client function.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the client function.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of what the client function does.\"\n    },\n    \"context\": {\n      \"type\": \"string\",\n      \"description\": \"The context path for organizing the function in the catalog.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n     \
  \ \"enum\": [\"typescript\", \"python\", \"java\", \"csharp\"],\n      \"description\": \"The programming language of the function.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The function source code.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\", \"deprecated\"],\n      \"description\": \"The lifecycle state of the function.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The owner of the function.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\"],\n      \"description\": \"The visibility of the function.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the function was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the function\
  \ was last updated.\"\n    }\n  },\n  \"required\": [\"name\", \"language\", \"code\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/json-schema/client-function.json
tags:
- Integrations
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
title: PolyAPI Client Function
---
