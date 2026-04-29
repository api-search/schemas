---
description: A datasets reference to an upstream task. *New in version 2.4.0*
layout: schema
name: TaskOutletDatasetReference
properties_list:
- description: The dataset creation time
  name: created_at
  type: string
- description: The DAG ID that updates the dataset.
  name: dag_id
  type: string
- description: The task ID that updates the dataset.
  name: task_id
  type: string
- description: The dataset update time
  name: updated_at
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-task-outlet-dataset-reference-schema.json
slug: openapi.yaml-task-outlet-dataset-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-outlet-dataset-reference-schema.json\",\n  \"title\": \"TaskOutletDatasetReference\",\n  \"description\": \"A datasets reference to an upstream task.\\n\\n*New in version 2.4.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_at\": {\n      \"description\": \"The dataset creation time\",\n      \"nullable\": false,\n      \"type\": \"string\"\n    },\n    \"dag_id\": {\n      \"description\": \"The DAG ID that updates the dataset.\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"task_id\": {\n      \"description\": \"The task ID that updates the dataset.\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"description\": \"The dataset update time\",\n      \"nullable\": false,\n      \"type\": \"string\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-outlet-dataset-reference-schema.json
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
title: TaskOutletDatasetReference
---
