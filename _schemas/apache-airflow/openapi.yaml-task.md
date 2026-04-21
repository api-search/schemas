---
description: 'For details see: [airflow.models.BaseOperator](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/index.html#airflow.models.BaseOperator)'
layout: schema
name: Task
properties_list:
- description: ''
  name: class_ref
  type: object
- description: ''
  name: depends_on_past
  type: boolean
- description: ''
  name: downstream_task_ids
  type: array
- description: ''
  name: end_date
  type: string
- description: ''
  name: execution_timeout
  type: object
- description: ''
  name: extra_links
  type: array
- description: ''
  name: is_mapped
  type: boolean
- description: ''
  name: owner
  type: string
- description: ''
  name: pool
  type: string
- description: ''
  name: pool_slots
  type: number
- description: ''
  name: priority_weight
  type: number
- description: ''
  name: queue
  type: string
- description: ''
  name: retries
  type: number
- description: ''
  name: retry_delay
  type: object
- description: ''
  name: retry_exponential_backoff
  type: boolean
- description: ''
  name: start_date
  type: string
- description: ''
  name: sub_dag
  type: object
- description: ''
  name: task_id
  type: string
- description: ''
  name: template_fields
  type: array
- description: ''
  name: trigger_rule
  type: object
- description: ''
  name: ui_color
  type: object
- description: ''
  name: ui_fgcolor
  type: object
- description: ''
  name: wait_for_downstream
  type: boolean
- description: ''
  name: weight_rule
  type: object
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-task-schema.json
slug: openapi.yaml-task
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
title: Task
---
