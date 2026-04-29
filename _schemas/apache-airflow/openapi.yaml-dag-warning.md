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
source_filename: openapi.yaml-dag-warning-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-warning-schema.json\",\n  \"title\": \"DagWarning\",\n  \"description\": \"DagWarning schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"description\": \"The dag_id.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"description\": \"The message for the dag warning.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"description\": \"The time when this warning was logged.\",\n      \"format\": \"datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"warning_type\": {\n      \"description\": \"The warning type for the dag warning.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-warning-schema.json
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
