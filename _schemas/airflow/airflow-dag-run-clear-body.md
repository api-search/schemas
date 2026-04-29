---
description: DAG Run serializer for clear endpoint body.
layout: schema
name: DAGRunClearBody
properties_list:
- description: ''
  name: dry_run
  type: boolean
- description: ''
  name: only_failed
  type: boolean
- description: (Experimental) Run on the latest bundle version of the Dag after clearing the Dag Run.
  name: run_on_latest_version
  type: boolean
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-run-clear-body-schema.json
slug: airflow-dag-run-clear-body
source_filename: airflow-dag-run-clear-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-clear-body-schema.json\",\n  \"title\": \"DAGRunClearBody\",\n  \"description\": \"DAG Run serializer for clear endpoint body.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dry_run\": {\n      \"type\": \"boolean\",\n      \"title\": \"Dry Run\",\n      \"default\": true\n    },\n    \"only_failed\": {\n      \"type\": \"boolean\",\n      \"title\": \"Only Failed\",\n      \"default\": false\n    },\n    \"run_on_latest_version\": {\n      \"type\": \"boolean\",\n      \"title\": \"Run On Latest Version\",\n      \"description\": \"(Experimental) Run on the latest bundle version of the Dag after clearing the Dag Run.\",\n      \"default\": false\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-clear-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DAGRunClearBody
---
