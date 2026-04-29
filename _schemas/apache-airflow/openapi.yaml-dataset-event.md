---
description: A dataset event. *New in version 2.4.0*
layout: schema
name: DatasetEvent
properties_list:
- description: ''
  name: created_dagruns
  type: array
- description: The dataset id
  name: dataset_id
  type: integer
- description: The URI of the dataset
  name: dataset_uri
  type: string
- description: The dataset event extra
  name: extra
  type: object
- description: The DAG ID that updated the dataset.
  name: source_dag_id
  type: string
- description: The task map index that updated the dataset.
  name: source_map_index
  type: integer
- description: The DAG run ID that updated the dataset.
  name: source_run_id
  type: string
- description: The task ID that updated the dataset.
  name: source_task_id
  type: string
- description: The dataset event creation time
  name: timestamp
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-dataset-event-schema.json
slug: openapi.yaml-dataset-event
source_filename: openapi.yaml-dataset-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dataset-event-schema.json\",\n  \"title\": \"DatasetEvent\",\n  \"description\": \"A dataset event.\\n\\n*New in version 2.4.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_dagruns\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BasicDAGRun\"\n      },\n      \"type\": \"array\"\n    },\n    \"dataset_id\": {\n      \"description\": \"The dataset id\",\n      \"type\": \"integer\"\n    },\n    \"dataset_uri\": {\n      \"description\": \"The URI of the dataset\",\n      \"nullable\": false,\n      \"type\": \"string\"\n    },\n    \"extra\": {\n      \"description\": \"The dataset event extra\",\n      \"nullable\": true,\n      \"type\": \"object\"\n    },\n    \"source_dag_id\": {\n      \"description\": \"The DAG ID that updated the dataset.\",\n\
  \      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"source_map_index\": {\n      \"description\": \"The task map index that updated the dataset.\",\n      \"nullable\": true,\n      \"type\": \"integer\"\n    },\n    \"source_run_id\": {\n      \"description\": \"The DAG run ID that updated the dataset.\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"source_task_id\": {\n      \"description\": \"The task ID that updated the dataset.\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"description\": \"The dataset event creation time\",\n      \"nullable\": false,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dataset-event-schema.json
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
title: DatasetEvent
---
