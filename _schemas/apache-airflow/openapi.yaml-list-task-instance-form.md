---
description: ListTaskInstanceForm schema from Apache Airflow API
layout: schema
name: ListTaskInstanceForm
properties_list:
- description: Return objects with specific DAG IDs. The value can be repeated to retrieve multiple matching values (OR condition).
  name: dag_ids
  type: array
- description: Returns objects greater than or equal to the specified values. This can be combined with duration_lte parameter to receive only the selected period.
  name: duration_gte
  type: number
- description: Returns objects less than or equal to the specified values. This can be combined with duration_gte parameter to receive only the selected range.
  name: duration_lte
  type: number
- description: Returns objects greater or equal the specified date. This can be combined with start_date_lte parameter to receive only the selected period.
  name: end_date_gte
  type: string
- description: Returns objects less than or equal to the specified date. This can be combined with start_date_gte parameter to receive only the selected period.
  name: end_date_lte
  type: string
- description: Returns objects greater or equal to the specified date. This can be combined with execution_date_lte parameter to receive only the selected period.
  name: execution_date_gte
  type: string
- description: Returns objects less than or equal to the specified date. This can be combined with execution_date_gte parameter to receive only the selected period.
  name: execution_date_lte
  type: string
- description: The value can be repeated to retrieve multiple matching values (OR condition).
  name: pool
  type: array
- description: The value can be repeated to retrieve multiple matching values (OR condition).
  name: queue
  type: array
- description: Returns objects greater or equal the specified date. This can be combined with start_date_lte parameter to receive only the selected period.
  name: start_date_gte
  type: string
- description: Returns objects less or equal the specified date. This can be combined with start_date_gte parameter to receive only the selected period.
  name: start_date_lte
  type: string
- description: The value can be repeated to retrieve multiple matching values (OR condition).
  name: state
  type: array
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-list-task-instance-form-schema.json
slug: openapi.yaml-list-task-instance-form
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
title: ListTaskInstanceForm
---
