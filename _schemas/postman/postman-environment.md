---
description: A Postman environment containing a set of key-value variable pairs that can be used across requests and collections. Environments enable you to scope your work to different contexts such as development, staging, and production.
layout: schema
name: Postman Environment
properties_list:
- description: The environment's unique identifier.
  name: id
  type: string
- description: The environment name as displayed in the Postman interface.
  name: name
  type: string
- description: The environment variables.
  name: values
  type: array
- description: The user ID of the environment owner.
  name: owner
  type: string
- description: The environment's UID in the format {ownerId}-{environmentId}.
  name: uid
  type: string
- description: The date and time when the environment was created.
  name: createdAt
  type: string
- description: The date and time when the environment was last updated.
  name: updatedAt
  type: string
- description: Whether the environment is publicly accessible.
  name: isPublic
  type: boolean
- description: Timestamp of when the environment was exported.
  name: _postman_exported_at
  type: string
- description: The Postman version used to export the environment.
  name: _postman_exported_using
  type: string
provider_name: Postman
provider_slug: postman
schema_file: json-schema/postman-environment-schema.json
slug: postman-environment
source_filename: postman-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://postman.com/schemas/postman/environment.json\",\n  \"title\": \"Postman Environment\",\n  \"description\": \"A Postman environment containing a set of key-value variable pairs that can be used across requests and collections. Environments enable you to scope your work to different contexts such as development, staging, and production.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"values\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The environment's unique identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The environment name as displayed in the Postman interface.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"The environment variables.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/EnvironmentVariable\"\n      }\n    },\n    \"owner\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The user ID of the environment owner.\"\n    },\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"The environment's UID in the format {ownerId}-{environmentId}.\",\n      \"pattern\": \"^[0-9]+-[a-zA-Z0-9-]+$\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the environment was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the environment was last updated.\"\n    },\n    \"isPublic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the environment is publicly accessible.\"\n    },\n    \"_postman_exported_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of when the environment was exported.\"\n    },\n    \"_postman_exported_using\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The Postman version used to export the environment.\"\n    }\n  },\n  \"$defs\": {\n    \"EnvironmentVariable\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value variable within the environment.\",\n      \"required\": [\"key\"],\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The variable name used for substitution in requests.\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The current value of the variable. For secret type variables, this may be masked.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"default\", \"secret\"],\n          \"description\": \"The variable type. Secret variables are masked in the UI and API responses.\",\n          \"default\": \"default\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\"\
  : \"Whether the variable is active. Disabled variables are not substituted in requests.\",\n          \"default\": true\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of what the variable is used for.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/postman/refs/heads/main/json-schema/postman-environment-schema.json
tags:
- AI Agent Builder
- API Development
- API Documentation
- API Governance
- API Monitoring
- API Testing
- Automation
- Client
- Clients
- Collaboration
- Collections
- Discovery
- Environments
- MCP
- Mock Servers
- Mocking
- Network
- Platform
- Testing
- Workflows
- Workspaces
title: Postman Environment
---
