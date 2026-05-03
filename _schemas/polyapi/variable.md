---
description: A variable or secret that is stored securely and injected into functions at runtime using a path identifier.
layout: schema
name: PolyAPI Variable
properties_list:
- description: The unique identifier of the variable.
  name: id
  type: string
- description: The name of the variable.
  name: name
  type: string
- description: A description of the variable.
  name: description
  type: string
- description: The path identifier used to reference this variable in functions (e.g., 'tutorial.apiKey').
  name: pathIdentifier
  type: string
- description: The variable value (masked for secrets).
  name: value
  type: string
- description: Whether this variable is stored as a secret.
  name: secret
  type: boolean
- description: The visibility of the variable.
  name: visibility
  type: string
- description: Timestamp when the variable was created.
  name: createdAt
  type: string
- description: Timestamp when the variable was last updated.
  name: updatedAt
  type: string
provider_name: PolyAPI
provider_slug: polyapi
schema_file: json-schema/variable.json
slug: variable
source_filename: variable.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/polyapi/blob/main/json-schema/variable.json\",\n  \"title\": \"PolyAPI Variable\",\n  \"description\": \"A variable or secret that is stored securely and injected into functions at runtime using a path identifier.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the variable.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the variable.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the variable.\"\n    },\n    \"pathIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The path identifier used to reference this variable in functions (e.g., 'tutorial.apiKey').\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The variable\
  \ value (masked for secrets).\"\n    },\n    \"secret\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether this variable is stored as a secret.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\"],\n      \"description\": \"The visibility of the variable.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the variable was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the variable was last updated.\"\n    }\n  },\n  \"required\": [\"name\", \"value\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/polyapi/refs/heads/main/json-schema/variable.json
tags:
- Integrations
- Microservices
- Middleware
- Orchestrations
- Pro-Code API Composition
title: PolyAPI Variable
---
