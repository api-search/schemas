---
description: Request body for creating a new mapping task.
layout: schema
name: MappingTaskCreateRequest
properties_list:
- description: The resource type identifier.
  name: '@type'
  type: string
- description: The name for the new mapping task.
  name: name
  type: string
- description: A description of the mapping task.
  name: description
  type: string
- description: The ID of the mapping to execute.
  name: mappingId
  type: string
- description: The runtime environment to use for execution.
  name: runtimeEnvironmentId
  type: string
- description: The schedule to associate with the task.
  name: scheduleId
  type: string
- description: The command to run before the task.
  name: preProcessingCmd
  type: string
- description: The command to run after the task.
  name: postProcessingCmd
  type: string
- description: The source connection ID.
  name: sourceConnectionId
  type: string
- description: The target connection ID.
  name: targetConnectionId
  type: string
- description: Parameter value overrides.
  name: parameters
  type: array
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-mapping-task-create-request-schema.json
slug: informatica-platform-rest-mapping-task-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MappingTaskCreateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new mapping task.\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the new mapping task.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the mapping task.\"\n    },\n    \"mappingId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the mapping to execute.\"\n    },\n    \"runtimeEnvironmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime environment to use for execution.\"\n    },\n    \"scheduleId\": {\n      \"type\": \"string\",\n      \"description\": \"The schedule to associate with the task.\"\n    },\n    \"preProcessingCmd\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The command to run before the task.\"\n    },\n    \"postProcessingCmd\": {\n      \"type\": \"string\",\n      \"description\": \"The command to run after the task.\"\n    },\n    \"sourceConnectionId\": {\n      \"type\": \"string\",\n      \"description\": \"The source connection ID.\"\n    },\n    \"targetConnectionId\": {\n      \"type\": \"string\",\n      \"description\": \"The target connection ID.\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"Parameter value overrides.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-mapping-task-create-request-schema.json
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
title: MappingTaskCreateRequest
---
