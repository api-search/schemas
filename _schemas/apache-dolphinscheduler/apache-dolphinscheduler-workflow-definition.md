---
description: A workflow (process) definition in Apache DolphinScheduler, representing a DAG of tasks.
layout: schema
name: WorkflowDefinition
properties_list:
- description: Unique workflow definition ID.
  name: id
  type: integer
- description: Globally unique code for the workflow definition.
  name: code
  type: integer
- description: Workflow definition name.
  name: name
  type: string
- description: Version number of this workflow definition.
  name: version
  type: integer
- description: Whether the workflow is online (released) or offline.
  name: releaseState
  type: string
- description: Code of the project this workflow belongs to.
  name: projectCode
  type: integer
- description: Human-readable description of the workflow.
  name: description
  type: string
- description: Global parameters for this workflow in JSON format.
  name: globalParams
  type: string
- description: Workflow execution timeout in minutes. 0 means no timeout.
  name: timeout
  type: integer
- description: Tenant code for resource isolation.
  name: tenantCode
  type: string
- description: ISO 8601 creation timestamp.
  name: createTime
  type: string
- description: ISO 8601 last update timestamp.
  name: updateTime
  type: string
provider_name: Apache DolphinScheduler
provider_slug: apache-dolphinscheduler
schema_file: json-schema/apache-dolphinscheduler-workflow-definition-schema.json
slug: apache-dolphinscheduler-workflow-definition
source_filename: apache-dolphinscheduler-workflow-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-dolphinscheduler/refs/heads/main/json-schema/apache-dolphinscheduler-workflow-definition-schema.json\",\n  \"title\": \"WorkflowDefinition\",\n  \"description\": \"A workflow (process) definition in Apache DolphinScheduler, representing a DAG of tasks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique workflow definition ID.\",\n      \"example\": 1001\n    },\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"Globally unique code for the workflow definition.\",\n      \"example\": 8888888888888\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Workflow definition name.\",\n      \"example\": \"daily-etl-pipeline\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Version number\
  \ of this workflow definition.\",\n      \"example\": 3\n    },\n    \"releaseState\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the workflow is online (released) or offline.\",\n      \"enum\": [\n        \"ONLINE\",\n        \"OFFLINE\"\n      ],\n      \"example\": \"ONLINE\"\n    },\n    \"projectCode\": {\n      \"type\": \"integer\",\n      \"description\": \"Code of the project this workflow belongs to.\",\n      \"example\": 7777777777777\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the workflow.\",\n      \"example\": \"Daily ETL pipeline for processing sales data\"\n    },\n    \"globalParams\": {\n      \"type\": \"string\",\n      \"description\": \"Global parameters for this workflow in JSON format.\",\n      \"example\": \"[]\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Workflow execution timeout in minutes. 0 means no timeout.\",\n     \
  \ \"example\": 60\n    },\n    \"tenantCode\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant code for resource isolation.\",\n      \"example\": \"etl-team\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 creation timestamp.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 last update timestamp.\",\n      \"example\": \"2025-03-20T10:00:00Z\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"projectCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-dolphinscheduler/refs/heads/main/json-schema/apache-dolphinscheduler-workflow-definition-schema.json
tags:
- Apache
- DAG
- Data Pipeline
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: WorkflowDefinition
---
