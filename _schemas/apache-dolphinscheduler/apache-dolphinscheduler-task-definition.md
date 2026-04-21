---
description: A task node in a DolphinScheduler workflow definition DAG.
layout: schema
name: TaskDefinition
properties_list:
- description: Task definition ID.
  name: id
  type: integer
- description: Globally unique task code.
  name: code
  type: integer
- description: Task name within the workflow.
  name: name
  type: string
- description: Task execution type.
  name: taskType
  type: string
- description: Task-specific parameters (structure varies by taskType).
  name: taskParams
  type: object
- description: Task description.
  name: description
  type: string
- description: Whether this task is enabled.
  name: flag
  type: string
- description: Task priority for scheduling.
  name: taskPriority
  type: string
- description: Worker group this task should run on.
  name: workerGroup
  type: string
- description: Number of retry attempts on failure.
  name: retryTimes
  type: integer
- description: Interval in minutes between retry attempts.
  name: retryInterval
  type: integer
- description: Task execution timeout in minutes.
  name: timeout
  type: integer
provider_name: Apache DolphinScheduler
provider_slug: apache-dolphinscheduler
schema_file: json-schema/apache-dolphinscheduler-task-definition-schema.json
slug: apache-dolphinscheduler-task-definition
tags:
- Apache
- DAG
- Data Pipeline
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: TaskDefinition
---
