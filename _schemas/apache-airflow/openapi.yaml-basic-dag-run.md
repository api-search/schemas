---
description: BasicDAGRun schema from Apache Airflow API
layout: schema
name: BasicDAGRun
properties_list:
- description: ''
  name: dag_id
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
- description: The logical date (previously called execution date). This is the time or interval covered by this DAG run, according to the DAG definition. The value of this field can be set only when creating the ob
  name: logical_date
  type: string
- description: Run ID.
  name: run_id
  type: string
- description: The start time. The time when DAG run was actually created. *Changed in version 2.1.3*&#58; Field becomes nullable.
  name: start_date
  type: string
- description: ''
  name: state
  type: object
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-basic-dag-run-schema.json
slug: openapi.yaml-basic-dag-run
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
title: BasicDAGRun
---
