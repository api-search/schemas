---
description: UpdateTaskInstance schema from Apache Airflow API
layout: schema
name: UpdateTaskInstance
properties_list:
- description: If set, don't actually run this operation. The response will contain the task instance planned to be affected, but won't be modified in any way.
  name: dry_run
  type: boolean
- description: Expected new state.
  name: new_state
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-update-task-instance-schema.json
slug: openapi.yaml-update-task-instance
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
title: UpdateTaskInstance
---
