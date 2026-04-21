---
description: ListDagRunsForm schema from Apache Airflow API
layout: schema
name: ListDagRunsForm
properties_list:
- description: Return objects with specific DAG IDs. The value can be repeated to retrieve multiple matching values (OR condition).
  name: dag_ids
  type: array
- description: Returns objects greater or equal the specified date. This can be combined with end_date_lte parameter to receive only the selected period.
  name: end_date_gte
  type: string
- description: Returns objects less than or equal to the specified date. This can be combined with end_date_gte parameter to receive only the selected period.
  name: end_date_lte
  type: string
- description: Returns objects greater or equal to the specified date. This can be combined with execution_date_lte key to receive only the selected period.
  name: execution_date_gte
  type: string
- description: Returns objects less than or equal to the specified date. This can be combined with execution_date_gte key to receive only the selected period.
  name: execution_date_lte
  type: string
- description: The name of the field to order the results by. Prefix a field name with `-` to reverse the sort order. *New in version 2.1.0*
  name: order_by
  type: string
- description: The numbers of items to return.
  name: page_limit
  type: integer
- description: The number of items to skip before starting to collect the result set.
  name: page_offset
  type: integer
- description: Returns objects greater or equal the specified date. This can be combined with start_date_lte key to receive only the selected period.
  name: start_date_gte
  type: string
- description: Returns objects less or equal the specified date. This can be combined with start_date_gte parameter to receive only the selected period
  name: start_date_lte
  type: string
- description: Return objects with specific states. The value can be repeated to retrieve multiple matching values (OR condition).
  name: states
  type: array
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-list-dag-runs-form-schema.json
slug: openapi.yaml-list-dag-runs-form
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
title: ListDagRunsForm
---
