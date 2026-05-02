---
description: A Neon operation tracks the progress of an action performed on a project resource such as creating a branch, starting a compute endpoint, or applying configuration changes.
layout: schema
name: Neon Operation
properties_list:
- description: The unique operation identifier
  name: id
  type: string
- description: The project ID this operation belongs to
  name: project_id
  type: string
- description: The branch ID associated with this operation, if applicable
  name: branch_id
  type: string
- description: The endpoint ID associated with this operation, if applicable
  name: endpoint_id
  type: string
- description: The type of action being performed by this operation
  name: action
  type: string
- description: The current status of the operation
  name: status
  type: string
- description: Number of times the operation has failed and been retried
  name: failures_count
  type: integer
- description: Error message if the operation failed
  name: error
  type: string
- description: Timestamp when the operation was created
  name: created_at
  type: string
- description: Timestamp when the operation status was last updated
  name: updated_at
  type: string
provider_name: Neon
provider_slug: neon
schema_file: json-schema/neon-operation-schema.json
slug: neon-operation
source_filename: neon-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://neon.com/schemas/neon/operation.json\",\n  \"title\": \"Neon Operation\",\n  \"description\": \"A Neon operation tracks the progress of an action performed on a project resource such as creating a branch, starting a compute endpoint, or applying configuration changes.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"project_id\", \"action\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique operation identifier\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"The project ID this operation belongs to\"\n    },\n    \"branch_id\": {\n      \"type\": \"string\",\n      \"description\": \"The branch ID associated with this operation, if applicable\"\n    },\n    \"endpoint_id\": {\n      \"type\": \"string\",\n      \"description\": \"The endpoint ID associated with this operation,\
  \ if applicable\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The type of action being performed by this operation\",\n      \"enum\": [\n        \"create_compute\",\n        \"create_timeline\",\n        \"start_compute\",\n        \"suspend_compute\",\n        \"apply_config\",\n        \"check_availability\",\n        \"delete_timeline\",\n        \"create_branch\",\n        \"tenant_ignore\",\n        \"tenant_attach\",\n        \"tenant_detach\",\n        \"replace_safekeeper\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the operation\",\n      \"enum\": [\n        \"scheduling\",\n        \"running\",\n        \"finished\",\n        \"failed\",\n        \"cancelling\",\n        \"cancelled\",\n        \"skipped\"\n      ]\n    },\n    \"failures_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times the operation has failed and been retried\",\n \
  \     \"minimum\": 0\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if the operation failed\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the operation was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the operation status was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/json-schema/neon-operation-schema.json
tags:
- Databases
- Serverless
- Postgres
- Infrastructure
- Authentication
- Edge
title: Neon Operation
---
