---
description: TaskInstance schema from Apache Airflow API
layout: schema
name: TaskInstance
properties_list:
- description: ''
  name: dag_id
  type: string
- description: The DagRun ID for this task instance *New in version 2.3.0*
  name: dag_run_id
  type: string
- description: ''
  name: duration
  type: number
- description: ''
  name: end_date
  type: string
- description: ''
  name: execution_date
  type: string
- description: ''
  name: executor_config
  type: string
- description: ''
  name: hostname
  type: string
- description: ''
  name: map_index
  type: integer
- description: ''
  name: max_tries
  type: integer
- description: Contains manually entered notes by the user about the TaskInstance. *New in version 2.5.0*
  name: note
  type: string
- description: '*Changed in version 2.1.1*&#58; Field becomes nullable.'
  name: operator
  type: string
- description: ''
  name: pid
  type: integer
- description: ''
  name: pool
  type: string
- description: ''
  name: pool_slots
  type: integer
- description: ''
  name: priority_weight
  type: integer
- description: ''
  name: queue
  type: string
- description: ''
  name: queued_when
  type: string
- description: JSON object describing rendered fields. *New in version 2.3.0*
  name: rendered_fields
  type: object
- description: ''
  name: sla_miss
  type: object
- description: ''
  name: start_date
  type: string
- description: ''
  name: state
  type: object
- description: ''
  name: task_id
  type: string
- description: ''
  name: trigger
  type: object
- description: ''
  name: triggerer_job
  type: object
- description: ''
  name: try_number
  type: integer
- description: ''
  name: unixname
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-task-instance-schema.json
slug: openapi.yaml-task-instance
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
title: TaskInstance
---
