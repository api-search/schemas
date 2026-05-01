---
description: Configuration for a function decorated with DBOS.workflow.
layout: schema
name: DBOS Workflow
properties_list:
- description: Stable workflow name used for tracking and recovery.
  name: name
  type: string
- description: Maximum recovery attempts after worker failure.
  name: max_recovery_attempts
  type: integer
- description: Argument serialization format.
  name: serialization_type
  type: string
- description: Whether to type-check arguments at runtime.
  name: validate_args
  type: boolean
provider_name: DBOS
provider_slug: dbos
schema_file: json-schema/workflow.json
slug: workflow
source_filename: workflow.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dbos/main/json-schema/workflow.json\",\n  \"title\": \"DBOS Workflow\",\n  \"description\": \"Configuration for a function decorated with DBOS.workflow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\"type\": \"string\", \"description\": \"Stable workflow name used for tracking and recovery.\"},\n    \"max_recovery_attempts\": {\"type\": \"integer\", \"minimum\": 0, \"description\": \"Maximum recovery attempts after worker failure.\"},\n    \"serialization_type\": {\"type\": \"string\", \"enum\": [\"json\", \"pickle\"], \"description\": \"Argument serialization format.\"},\n    \"validate_args\": {\"type\": \"boolean\", \"description\": \"Whether to type-check arguments at runtime.\"}\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dbos/refs/heads/main/json-schema/workflow.json
tags:
- API Composition
- Durable Execution
- Postgres
- Queues
- Scheduled Jobs
- Workflow
title: DBOS Workflow
---
