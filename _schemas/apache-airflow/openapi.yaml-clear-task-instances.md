---
description: ClearTaskInstances schema from Apache Airflow API
layout: schema
name: ClearTaskInstances
properties_list:
- description: The DagRun ID for this task instance
  name: dag_run_id
  type: string
- description: If set, don't actually run this operation. The response will contain a list of task instances planned to be cleaned, but not modified in any way.
  name: dry_run
  type: boolean
- description: The maximum execution date to clear.
  name: end_date
  type: string
- description: If set to true, downstream tasks are also affected.
  name: include_downstream
  type: boolean
- description: If set to True, also tasks from future DAG Runs are affected.
  name: include_future
  type: boolean
- description: Clear tasks in the parent dag of the subdag.
  name: include_parentdag
  type: boolean
- description: If set to True, also tasks from past DAG Runs are affected.
  name: include_past
  type: boolean
- description: Clear tasks in subdags and clear external tasks indicated by ExternalTaskMarker.
  name: include_subdags
  type: boolean
- description: If set to true, upstream tasks are also affected.
  name: include_upstream
  type: boolean
- description: Only clear failed tasks.
  name: only_failed
  type: boolean
- description: Only clear running tasks.
  name: only_running
  type: boolean
- description: Set state of DAG runs to RUNNING.
  name: reset_dag_runs
  type: boolean
- description: The minimum execution date to clear.
  name: start_date
  type: string
- description: A list of task ids to clear. *New in version 2.1.0*
  name: task_ids
  type: array
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-clear-task-instances-schema.json
slug: openapi.yaml-clear-task-instances
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
title: ClearTaskInstances
---
