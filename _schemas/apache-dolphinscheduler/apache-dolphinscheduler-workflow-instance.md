---
description: A running or completed instance of a workflow definition in Apache DolphinScheduler.
layout: schema
name: WorkflowInstance
properties_list:
- description: Unique workflow instance ID.
  name: id
  type: integer
- description: Code of the workflow definition that created this instance.
  name: processDefinitionCode
  type: integer
- description: Workflow instance name (typically includes a timestamp).
  name: name
  type: string
- description: Execution state of this workflow instance.
  name: state
  type: string
- description: Execution start time.
  name: startTime
  type: string
- description: Execution end time (null if still running).
  name: endTime
  type: string
- description: Human-readable execution duration.
  name: duration
  type: string
- description: Number of times this instance has been re-run.
  name: runTimes
  type: integer
- description: Type of command that triggered this instance.
  name: commandType
  type: string
- description: Worker host that is executing this instance.
  name: host
  type: string
provider_name: Apache DolphinScheduler
provider_slug: apache-dolphinscheduler
schema_file: json-schema/apache-dolphinscheduler-workflow-instance-schema.json
slug: apache-dolphinscheduler-workflow-instance
tags:
- Apache
- DAG
- Data Pipeline
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: WorkflowInstance
---
