---
description: A Neon compute endpoint provides the processing resources for executing database queries against a branch. Each branch supports one read-write endpoint and multiple read-only endpoints with configurable autoscaling.
layout: schema
name: Neon Compute Endpoint
properties_list:
- description: The unique endpoint identifier
  name: id
  type: string
- description: The hostname for connecting to this endpoint
  name: host
  type: string
- description: The project ID this endpoint belongs to
  name: project_id
  type: string
- description: The branch ID this endpoint is attached to
  name: branch_id
  type: string
- description: The cloud region where this endpoint is deployed
  name: region_id
  type: string
- description: Minimum compute units for autoscaling
  name: autoscaling_limit_min_cu
  type: number
- description: Maximum compute units for autoscaling
  name: autoscaling_limit_max_cu
  type: number
- description: The endpoint type determining read/write access
  name: type
  type: string
- description: The current operational state of the endpoint
  name: current_state
  type: string
- description: Seconds of inactivity before the endpoint is automatically suspended to save resources
  name: suspend_timeout_seconds
  type: integer
- description: The provisioner type used for this endpoint
  name: provisioner
  type: string
- description: Whether the endpoint is disabled
  name: disabled
  type: boolean
- description: Timestamp when the endpoint was created
  name: created_at
  type: string
- description: Timestamp when the endpoint was last updated
  name: updated_at
  type: string
provider_name: Neon
provider_slug: neon
schema_file: json-schema/neon-endpoint-schema.json
slug: neon-endpoint
source_filename: neon-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://neon.com/schemas/neon/endpoint.json\",\n  \"title\": \"Neon Compute Endpoint\",\n  \"description\": \"A Neon compute endpoint provides the processing resources for executing database queries against a branch. Each branch supports one read-write endpoint and multiple read-only endpoints with configurable autoscaling.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"project_id\", \"branch_id\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique endpoint identifier\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname for connecting to this endpoint\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"description\": \"The project ID this endpoint belongs to\"\n    },\n    \"branch_id\": {\n      \"type\": \"string\",\n      \"description\": \"The branch ID this endpoint\
  \ is attached to\"\n    },\n    \"region_id\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud region where this endpoint is deployed\"\n    },\n    \"autoscaling_limit_min_cu\": {\n      \"type\": \"number\",\n      \"description\": \"Minimum compute units for autoscaling\",\n      \"minimum\": 0.25\n    },\n    \"autoscaling_limit_max_cu\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum compute units for autoscaling\",\n      \"minimum\": 0.25\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The endpoint type determining read/write access\",\n      \"enum\": [\"read_write\", \"read_only\"]\n    },\n    \"current_state\": {\n      \"type\": \"string\",\n      \"description\": \"The current operational state of the endpoint\",\n      \"enum\": [\"init\", \"active\", \"idle\"]\n    },\n    \"suspend_timeout_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds of inactivity before the endpoint is\
  \ automatically suspended to save resources\",\n      \"minimum\": 0\n    },\n    \"provisioner\": {\n      \"type\": \"string\",\n      \"description\": \"The provisioner type used for this endpoint\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the endpoint is disabled\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the endpoint was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the endpoint was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/json-schema/neon-endpoint-schema.json
tags:
- Databases
- Serverless
- Postgres
- Infrastructure
- Authentication
- Edge
title: Neon Compute Endpoint
---
