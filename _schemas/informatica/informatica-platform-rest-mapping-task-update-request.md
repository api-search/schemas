---
description: Request body for updating an existing mapping task.
layout: schema
name: MappingTaskUpdateRequest
properties_list:
- description: The resource type identifier.
  name: '@type'
  type: string
- description: The updated name.
  name: name
  type: string
- description: The updated description.
  name: description
  type: string
- description: The updated runtime environment.
  name: runtimeEnvironmentId
  type: string
- description: The updated schedule ID.
  name: scheduleId
  type: string
- description: The updated pre-processing command.
  name: preProcessingCmd
  type: string
- description: The updated post-processing command.
  name: postProcessingCmd
  type: string
- description: The updated source connection ID.
  name: sourceConnectionId
  type: string
- description: The updated target connection ID.
  name: targetConnectionId
  type: string
- description: Updated parameter values.
  name: parameters
  type: array
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-mapping-task-update-request-schema.json
slug: informatica-platform-rest-mapping-task-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MappingTaskUpdateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating an existing mapping task.\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The updated name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The updated description.\"\n    },\n    \"runtimeEnvironmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The updated runtime environment.\"\n    },\n    \"scheduleId\": {\n      \"type\": \"string\",\n      \"description\": \"The updated schedule ID.\"\n    },\n    \"preProcessingCmd\": {\n      \"type\": \"string\",\n      \"description\": \"The updated pre-processing command.\"\n    },\n    \"postProcessingCmd\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The updated post-processing command.\"\n    },\n    \"sourceConnectionId\": {\n      \"type\": \"string\",\n      \"description\": \"The updated source connection ID.\"\n    },\n    \"targetConnectionId\": {\n      \"type\": \"string\",\n      \"description\": \"The updated target connection ID.\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"Updated parameter values.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-mapping-task-update-request-schema.json
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
title: MappingTaskUpdateRequest
---
