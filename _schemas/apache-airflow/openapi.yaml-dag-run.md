---
description: DAGRun schema from Apache Airflow API
layout: schema
name: DAGRun
properties_list:
- description: JSON object describing additional configuration parameters. The value of this field can be set only when creating the object. If you try to modify the field of an existing object, the request fails wi
  name: conf
  type: object
- description: ''
  name: dag_id
  type: string
- description: Run ID. The value of this field can be set only when creating the object. If you try to modify the field of an existing object, the request fails with an BAD_REQUEST error. If not provided, a value wi
  name: dag_run_id
  type: string
- description: ''
  name: data_interval_end
  type: string
- description: ''
  name: data_interval_start
  type: string
- description: ''
  name: end_date
  type: string
- description: The execution date. This is the same as logical_date, kept for backwards compatibility. If both this field and logical_date are provided but with different values, the request will fail with an BAD_RE
  name: execution_date
  type: string
- description: ''
  name: external_trigger
  type: boolean
- description: ''
  name: last_scheduling_decision
  type: string
- description: The logical date (previously called execution date). This is the time or interval covered by this DAG run, according to the DAG definition. The value of this field can be set only when creating the ob
  name: logical_date
  type: string
- description: Contains manually entered notes by the user about the DagRun. *New in version 2.5.0*
  name: note
  type: string
- description: ''
  name: run_type
  type: string
- description: The start time. The time when DAG run was actually created. *Changed in version 2.1.3*&#58; Field becomes nullable.
  name: start_date
  type: string
- description: ''
  name: state
  type: object
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-dag-run-schema.json
slug: openapi.yaml-dag-run
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
title: DAGRun
---
