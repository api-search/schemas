---
description: Represents a mapping task that executes a mapping with specific source and target connections and runtime parameters.
layout: schema
name: MappingTask
properties_list:
- description: The resource type identifier.
  name: '@type'
  type: string
- description: The unique identifier for the mapping task.
  name: id
  type: string
- description: The organization ID that owns the task.
  name: orgId
  type: string
- description: The name of the mapping task.
  name: name
  type: string
- description: A description of the mapping task.
  name: description
  type: string
- description: The time the mapping task was created.
  name: createTime
  type: string
- description: The time the mapping task was last updated.
  name: updateTime
  type: string
- description: The user who created the mapping task.
  name: createdBy
  type: string
- description: The user who last updated the mapping task.
  name: updatedBy
  type: string
- description: The ID of the mapping that this task executes.
  name: mappingId
  type: string
- description: The runtime environment to use for execution.
  name: runtimeEnvironmentId
  type: string
- description: The schedule ID if the task is scheduled.
  name: scheduleId
  type: string
- description: The command to run before the task executes.
  name: preProcessingCmd
  type: string
- description: The command to run after the task executes.
  name: postProcessingCmd
  type: string
- description: The parameter values for this task execution. Overrides default mapping parameters.
  name: parameters
  type: array
- description: The source connection ID for the mapping task.
  name: sourceConnectionId
  type: string
- description: The target connection ID for the mapping task.
  name: targetConnectionId
  type: string
- description: The federated task ID.
  name: frsId
  type: string
- description: Whether the mapping task is active.
  name: active
  type: boolean
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-mapping-task-schema.json
slug: informatica-platform-rest-mapping-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MappingTask\",\n  \"type\": \"object\",\n  \"description\": \"Represents a mapping task that executes a mapping with specific source and target connections and runtime parameters.\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the mapping task.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"The organization ID that owns the task.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the mapping task.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the mapping task.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the mapping task\
  \ was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the mapping task was last updated.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who created the mapping task.\"\n    },\n    \"updatedBy\": {\n      \"type\": \"string\",\n      \"description\": \"The user who last updated the mapping task.\"\n    },\n    \"mappingId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the mapping that this task executes.\"\n    },\n    \"runtimeEnvironmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The runtime environment to use for execution.\"\n    },\n    \"scheduleId\": {\n      \"type\": \"string\",\n      \"description\": \"The schedule ID if the task is scheduled.\"\n    },\n    \"preProcessingCmd\": {\n      \"type\": \"string\",\n      \"description\": \"The command to run before the task executes.\"\n    },\n    \"postProcessingCmd\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The command to run after the task executes.\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"The parameter values for this task execution. Overrides default mapping parameters.\"\n    },\n    \"sourceConnectionId\": {\n      \"type\": \"string\",\n      \"description\": \"The source connection ID for the mapping task.\"\n    },\n    \"targetConnectionId\": {\n      \"type\": \"string\",\n      \"description\": \"The target connection ID for the mapping task.\"\n    },\n    \"frsId\": {\n      \"type\": \"string\",\n      \"description\": \"The federated task ID.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the mapping task is active.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-mapping-task-schema.json
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
title: MappingTask
---
