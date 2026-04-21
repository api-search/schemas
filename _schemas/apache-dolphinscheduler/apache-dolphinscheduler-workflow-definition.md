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
