---
description: SLAMiss schema from Apache Airflow API
layout: schema
name: SLAMiss
properties_list:
- description: The DAG ID.
  name: dag_id
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: email_sent
  type: boolean
- description: ''
  name: execution_date
  type: string
- description: ''
  name: notification_sent
  type: boolean
- description: The task ID.
  name: task_id
  type: string
- description: ''
  name: timestamp
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-sla-miss-schema.json
slug: openapi.yaml-sla-miss
source_filename: openapi.yaml-sla-miss-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-sla-miss-schema.json\",\n  \"title\": \"SLAMiss\",\n  \"description\": \"SLAMiss schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"description\": \"The DAG ID.\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"email_sent\": {\n      \"type\": \"boolean\"\n    },\n    \"execution_date\": {\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    },\n    \"notification_sent\": {\n      \"type\": \"boolean\"\n    },\n    \"task_id\": {\n      \"description\": \"The task ID.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-sla-miss-schema.json
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
title: SLAMiss
---
