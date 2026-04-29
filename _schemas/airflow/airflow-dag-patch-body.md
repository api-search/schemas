---
description: Dag Serializer for updatable bodies.
layout: schema
name: DAGPatchBody
properties_list:
- description: ''
  name: is_paused
  type: boolean
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-patch-body-schema.json
slug: airflow-dag-patch-body
source_filename: airflow-dag-patch-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-patch-body-schema.json\",\n  \"title\": \"DAGPatchBody\",\n  \"description\": \"Dag Serializer for updatable bodies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"is_paused\": {\n      \"type\": \"boolean\",\n      \"title\": \"Is Paused\"\n    }\n  },\n  \"required\": [\n    \"is_paused\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-patch-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DAGPatchBody
---
