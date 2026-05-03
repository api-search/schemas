---
description: A project represents an application or service within a Prisma workspace. Projects contain environments with database connections and API keys, and serve as the primary organizational unit for Prisma Data Platform resources.
layout: schema
name: Prisma Project
properties_list:
- description: Unique identifier for the project
  name: id
  type: string
- description: Display name of the project
  name: name
  type: string
- description: Identifier of the parent workspace
  name: workspaceId
  type: string
- description: Deployment environments configured for the project
  name: environments
  type: array
- description: Prisma Postgres databases associated with the project
  name: databases
  type: array
- description: ISO 8601 timestamp when the project was created
  name: createdAt
  type: string
- description: ISO 8601 timestamp when the project was last updated
  name: updatedAt
  type: string
provider_name: Prisma
provider_slug: prisma
schema_file: json-schema/prisma-project-schema.json
slug: prisma-project
source_filename: prisma-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://prisma.io/schemas/project.json\",\n  \"title\": \"Prisma Project\",\n  \"description\": \"A project represents an application or service within a Prisma workspace. Projects contain environments with database connections and API keys, and serve as the primary organizational unit for Prisma Data Platform resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the project\",\n      \"examples\": [\"prj_abc123def456\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the project\",\n      \"minLength\": 1,\n      \"maxLength\": 255,\n      \"examples\": [\"My Application\"]\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the parent workspace\"\n    },\n    \"environments\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"Deployment environments configured for the project\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Environment\"\n      }\n    },\n    \"databases\": {\n      \"type\": \"array\",\n      \"description\": \"Prisma Postgres databases associated with the project\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DatabaseReference\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the project was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the project was last updated\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"workspaceId\", \"createdAt\", \"updatedAt\"],\n  \"additionalProperties\": false,\n  \"$defs\": {\n    \"Environment\": {\n      \"type\": \"object\",\n      \"description\": \"A deployment environment within a project representing a\
  \ stage such as development, staging, or production\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the environment\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the environment\",\n          \"examples\": [\"Production\", \"Staging\", \"Development\"]\n        },\n        \"projectId\": {\n          \"type\": \"string\",\n          \"description\": \"Identifier of the parent project\"\n        },\n        \"connectionString\": {\n          \"type\": \"string\",\n          \"description\": \"Database connection string for this environment\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the environment was created\"\n        },\n        \"updatedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\
  ,\n          \"description\": \"ISO 8601 timestamp when the environment was last updated\"\n        }\n      },\n      \"required\": [\"id\", \"name\", \"projectId\", \"createdAt\", \"updatedAt\"]\n    },\n    \"DatabaseReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a Prisma Postgres database associated with the project\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the database\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"Region where the database is deployed\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current operational status\",\n          \"enum\": [\"provisioning\", \"active\", \"suspended\", \"deleting\", \"deleted\"]\n        }\n      },\n      \"required\": [\"id\", \"region\", \"status\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prisma/refs/heads/main/json-schema/prisma-project-schema.json
tags: []
title: Prisma Project
---
