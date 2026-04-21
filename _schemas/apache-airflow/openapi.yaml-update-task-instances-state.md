---
description: UpdateTaskInstancesState schema from Apache Airflow API
layout: schema
name: UpdateTaskInstancesState
properties_list:
- description: The task instance's DAG run ID. Either set this or execution_date but not both. *New in version 2.3.0*
  name: dag_run_id
  type: string
- description: If set, don't actually run this operation. The response will contain a list of task instances planned to be affected, but won't be modified in any way.
  name: dry_run
  type: boolean
- description: The execution date. Either set this or dag_run_id but not both.
  name: execution_date
  type: string
- description: If set to true, downstream tasks are also affected.
  name: include_downstream
  type: boolean
- description: If set to True, also tasks from future DAG Runs are affected.
  name: include_future
  type: boolean
- description: If set to True, also tasks from past DAG Runs are affected.
  name: include_past
  type: boolean
- description: If set to true, upstream tasks are also affected.
  name: include_upstream
  type: boolean
- description: Expected new state.
  name: new_state
  type: string
- description: The task ID.
  name: task_id
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-update-task-instances-state-schema.json
slug: openapi.yaml-update-task-instances-state
tags:
- Apache
- DAG
- Data Pipeline
- ETL
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: UpdateTaskInstancesState
---
