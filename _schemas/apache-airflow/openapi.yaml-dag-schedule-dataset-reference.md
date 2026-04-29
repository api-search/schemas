---
description: A datasets reference to a downstream DAG. *New in version 2.4.0*
layout: schema
name: DagScheduleDatasetReference
properties_list:
- description: The dataset reference creation time
  name: created_at
  type: string
- description: The DAG ID that depends on the dataset.
  name: dag_id
  type: string
- description: The dataset reference update time
  name: updated_at
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-dag-schedule-dataset-reference-schema.json
slug: openapi.yaml-dag-schedule-dataset-reference
source_filename: openapi.yaml-dag-schedule-dataset-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-schedule-dataset-reference-schema.json\",\n  \"title\": \"DagScheduleDatasetReference\",\n  \"description\": \"A datasets reference to a downstream DAG.\\n\\n*New in version 2.4.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_at\": {\n      \"description\": \"The dataset reference creation time\",\n      \"nullable\": false,\n      \"type\": \"string\"\n    },\n    \"dag_id\": {\n      \"description\": \"The DAG ID that depends on the dataset.\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"description\": \"The dataset reference update time\",\n      \"nullable\": false,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-schedule-dataset-reference-schema.json
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
title: DagScheduleDatasetReference
---
