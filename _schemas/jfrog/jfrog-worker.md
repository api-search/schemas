---
description: Represents a serverless worker in the JFrog Platform that extends platform functionality through synchronized hooks and automation. Workers are TypeScript-based functions that react to JFrog Platform events in a secure, isolated execution environment.
layout: schema
name: JFrog Worker
properties_list:
- description: Unique worker key identifier
  name: key
  type: string
- description: Human-readable description of the worker's purpose
  name: description
  type: string
- description: Whether the worker is currently active
  name: enabled
  type: boolean
- description: TypeScript source code for the worker
  name: source_code
  type: string
- description: The JFrog Platform event that triggers this worker
  name: action
  type: string
- description: Criteria for filtering which events trigger the worker
  name: filter_criteria
  type: object
- description: Encrypted secrets accessible to the worker at runtime
  name: secrets
  type: array
- description: Worker creation timestamp
  name: created
  type: string
- description: Last modification timestamp
  name: modified
  type: string
provider_name: JFrog
provider_slug: jfrog
schema_file: json-schema/jfrog-worker-schema.json
slug: jfrog-worker
source_filename: jfrog-worker-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/worker\",\n  \"title\": \"JFrog Worker\",\n  \"description\": \"Represents a serverless worker in the JFrog Platform that extends platform functionality through synchronized hooks and automation. Workers are TypeScript-based functions that react to JFrog Platform events in a secure, isolated execution environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Unique worker key identifier\",\n      \"examples\": [\n        \"my-download-validator\",\n        \"artifact-scanner\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the worker's purpose\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the worker is currently active\",\n      \"default\": true\n    },\n    \"source_code\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"TypeScript source code for the worker\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The JFrog Platform event that triggers this worker\",\n      \"enum\": [\n        \"BEFORE_DOWNLOAD\",\n        \"AFTER_DOWNLOAD\",\n        \"BEFORE_UPLOAD\",\n        \"AFTER_CREATE\",\n        \"AFTER_BUILD_INFO_SAVE\",\n        \"AFTER_MOVE\",\n        \"AFTER_COPY\",\n        \"BEFORE_DELETE\",\n        \"BEFORE_CREATE_TOKEN\",\n        \"GENERIC_EVENT\"\n      ]\n    },\n    \"filter_criteria\": {\n      \"type\": \"object\",\n      \"description\": \"Criteria for filtering which events trigger the worker\",\n      \"properties\": {\n        \"artifact_filter_criteria\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"repo_keys\": {\n              \"type\": \"array\",\n              \"description\": \"Repository keys to scope the worker to\",\n              \"items\": {\n\
  \                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"secrets\": {\n      \"type\": \"array\",\n      \"description\": \"Encrypted secrets accessible to the worker at runtime\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"Secret key name\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"Secret value (write-only, not returned in GET)\"\n          }\n        },\n        \"required\": [\n          \"key\"\n        ]\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Worker creation timestamp\"\n    },\n    \"modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    }\n  },\n  \"required\": [\n   \
  \ \"key\",\n    \"source_code\",\n    \"action\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/json-schema/jfrog-worker-schema.json
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
title: JFrog Worker
---
