---
description: A dataset event. *New in version 2.4.0*
layout: schema
name: DatasetEvent
properties_list:
- description: ''
  name: created_dagruns
  type: array
- description: The dataset id
  name: dataset_id
  type: integer
- description: The URI of the dataset
  name: dataset_uri
  type: string
- description: The dataset event extra
  name: extra
  type: object
- description: The DAG ID that updated the dataset.
  name: source_dag_id
  type: string
- description: The task map index that updated the dataset.
  name: source_map_index
  type: integer
- description: The DAG run ID that updated the dataset.
  name: source_run_id
  type: string
- description: The task ID that updated the dataset.
  name: source_task_id
  type: string
- description: The dataset event creation time
  name: timestamp
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-dataset-event-schema.json
slug: openapi.yaml-dataset-event
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
title: DatasetEvent
---
