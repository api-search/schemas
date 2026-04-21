---
description: DagWarning schema from Apache Airflow API
layout: schema
name: DagWarning
properties_list:
- description: The dag_id.
  name: dag_id
  type: string
- description: The message for the dag warning.
  name: message
  type: string
- description: The time when this warning was logged.
  name: timestamp
  type: string
- description: The warning type for the dag warning.
  name: warning_type
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-dag-warning-schema.json
slug: openapi.yaml-dag-warning
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
title: DagWarning
---
