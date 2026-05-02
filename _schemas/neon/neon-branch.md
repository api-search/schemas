---
description: A Neon branch is a copy-on-write clone of database data used for development, testing, or preview environments. Branches are created instantly and share storage with their parent until data diverges.
layout: schema
name: Neon Branch
properties_list:
- description: The unique branch identifier
  name: id
  type: string
- description: The project ID this branch belongs to
  name: project_id
  type: string
- description: The parent branch ID this branch was created from
  name: parent_id
  type: string
- description: The Postgres Log Sequence Number of the point the branch was created from
  name: parent_lsn
  type: string
- description: The timestamp of the point in time the branch was created from
  name: parent_timestamp
  type: string
- description: The human-readable branch name
  name: name
  type: string
- description: The current state of the branch
  name: current_state
  type: string
- description: The logical size of the branch data in bytes
  name: logical_size
  type: integer
- description: Whether this is the primary (default) branch of the project
  name: primary
  type: boolean
- description: Timestamp when the branch was created
  name: created_at
  type: string
- description: Timestamp when the branch was last updated
  name: updated_at
  type: string
provider_name: Neon
provider_slug: neon
schema_file: json-schema/neon-branch-schema.json
slug: neon-branch
source_filename: neon-branch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://neon.com/schemas/neon/branch.json\",\n  \"title\": \"Neon Branch\",\n  \"description\": \"A Neon branch is a copy-on-write clone of database data used for development, testing, or preview environments. Branches are created instantly and share storage with their parent until data diverges.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"project_id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique branch identifier\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"The project ID this branch belongs to\"\n    },\n    \"parent_id\": {\n      \"type\": \"string\",\n      \"description\": \"The parent branch ID this branch was created from\"\n    },\n    \"parent_lsn\": {\n      \"type\": \"string\",\n      \"description\": \"The Postgres Log Sequence Number of the point the branch\
  \ was created from\"\n    },\n    \"parent_timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp of the point in time the branch was created from\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable branch name\"\n    },\n    \"current_state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the branch\",\n      \"enum\": [\"init\", \"ready\"]\n    },\n    \"logical_size\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The logical size of the branch data in bytes\",\n      \"minimum\": 0\n    },\n    \"primary\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the primary (default) branch of the project\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the branch was created\"\n    },\n    \"updated_at\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the branch was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/json-schema/neon-branch-schema.json
tags:
- Databases
- Serverless
- Postgres
- Infrastructure
- Authentication
- Edge
title: Neon Branch
---
