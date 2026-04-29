---
description: Object used for create backfill request.
layout: schema
name: BackfillPostBody
properties_list:
- description: ''
  name: dag_id
  type: string
- description: ''
  name: from_date
  type: string
- description: ''
  name: to_date
  type: string
- description: ''
  name: run_backwards
  type: boolean
- description: ''
  name: dag_run_conf
  type: object
- description: ''
  name: reprocess_behavior
  type: object
- description: ''
  name: max_active_runs
  type: integer
- description: ''
  name: run_on_latest_version
  type: boolean
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-backfill-post-body-schema.json
slug: airflow-backfill-post-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-backfill-post-body-schema.json\",\n  \"title\": \"BackfillPostBody\",\n  \"description\": \"Object used for create backfill request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"from_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"From Date\"\n    },\n    \"to_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"To Date\"\n    },\n    \"run_backwards\": {\n      \"type\": \"boolean\",\n      \"title\": \"Run Backwards\",\n      \"default\": false\n    },\n    \"dag_run_conf\": {\n      \"additionalProperties\": true,\n      \"type\": \"object\",\n      \"title\": \"Dag Run Conf\",\n      \"default\": {}\n    },\n    \"reprocess_behavior\"\
  : {\n      \"$ref\": \"#/components/schemas/ReprocessBehavior\",\n      \"default\": \"none\"\n    },\n    \"max_active_runs\": {\n      \"type\": \"integer\",\n      \"title\": \"Max Active Runs\",\n      \"default\": 10\n    },\n    \"run_on_latest_version\": {\n      \"type\": \"boolean\",\n      \"title\": \"Run On Latest Version\",\n      \"default\": true\n    }\n  },\n  \"required\": [\n    \"dag_id\",\n    \"from_date\",\n    \"to_date\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-backfill-post-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: BackfillPostBody
---
