---
description: An Insomnia environment stores key-value pairs of variables that can be referenced in requests using template tags. Environments allow switching between different configurations such as development, staging, and production without modifying individual requests.
layout: schema
name: Insomnia Environment
properties_list:
- description: Unique identifier for the environment, typically prefixed with env_.
  name: _id
  type: string
- description: Human-readable name of the environment (e.g., Development, Staging, Production).
  name: name
  type: string
- description: Key-value pairs of environment variables available for template tag substitution in requests.
  name: data
  type: object
- description: Defines the display order of data properties in the UI.
  name: dataPropertyOrder
  type:
  - object
  - 'null'
- description: Optional color code for visual identification of the environment in the UI.
  name: color
  type:
  - string
  - 'null'
- description: Identifier of the parent workspace or base environment.
  name: parentId
  type: string
- description: Sort key used for ordering environments in the UI.
  name: metaSortKey
  type: integer
- description: Whether the environment is private and excluded from cloud sync and Git storage. Useful for storing secrets locally.
  name: isPrivate
  type: boolean
- description: Unix timestamp in milliseconds when the environment was created.
  name: created
  type: integer
- description: Unix timestamp in milliseconds when the environment was last modified.
  name: modified
  type: integer
- description: The resource type identifier.
  name: _type
  type: string
provider_name: Insomnia
provider_slug: insomnia
schema_file: json-schema/environment.json
slug: environment
source_filename: environment.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/json-schema/environment.json\",\n  \"title\": \"Insomnia Environment\",\n  \"description\": \"An Insomnia environment stores key-value pairs of variables that can be referenced in requests using template tags. Environments allow switching between different configurations such as development, staging, and production without modifying individual requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the environment, typically prefixed with env_.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the environment (e.g., Development, Staging, Production).\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs of environment variables available\
  \ for template tag substitution in requests.\",\n      \"additionalProperties\": {\n        \"description\": \"Environment variable value, which can be a string, number, boolean, object, or array.\"\n      }\n    },\n    \"dataPropertyOrder\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Defines the display order of data properties in the UI.\",\n      \"properties\": {\n        \"&\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Ordered list of property keys.\"\n        }\n      }\n    },\n    \"color\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Optional color code for visual identification of the environment in the UI.\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the parent workspace or base environment.\"\n    },\n    \"metaSortKey\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Sort key used for ordering environments in the UI.\"\n    },\n    \"isPrivate\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the environment is private and excluded from cloud sync and Git storage. Useful for storing secrets locally.\",\n      \"default\": false\n    },\n    \"created\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in milliseconds when the environment was created.\"\n    },\n    \"modified\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in milliseconds when the environment was last modified.\"\n    },\n    \"_type\": {\n      \"type\": \"string\",\n      \"const\": \"environment\",\n      \"description\": \"The resource type identifier.\"\n    }\n  },\n  \"required\": [\"_id\", \"name\", \"data\", \"parentId\", \"_type\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/json-schema/environment.json
tags:
- API Design
- CLI
- Clients
- Mocking
- Platform
- Testing
title: Insomnia Environment
---
