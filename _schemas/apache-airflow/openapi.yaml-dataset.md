---
description: A dataset item. *New in version 2.4.0*
layout: schema
name: Dataset
properties_list:
- description: ''
  name: consuming_dags
  type: array
- description: The dataset creation time
  name: created_at
  type: string
- description: The dataset extra
  name: extra
  type: object
- description: The dataset id
  name: id
  type: integer
- description: ''
  name: producing_tasks
  type: array
- description: The dataset update time
  name: updated_at
  type: string
- description: The dataset uri
  name: uri
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-dataset-schema.json
slug: openapi.yaml-dataset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dataset-schema.json\",\n  \"title\": \"Dataset\",\n  \"description\": \"A dataset item.\\n\\n*New in version 2.4.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"consuming_dags\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DagScheduleDatasetReference\"\n      },\n      \"type\": \"array\"\n    },\n    \"created_at\": {\n      \"description\": \"The dataset creation time\",\n      \"nullable\": false,\n      \"type\": \"string\"\n    },\n    \"extra\": {\n      \"description\": \"The dataset extra\",\n      \"nullable\": true,\n      \"type\": \"object\"\n    },\n    \"id\": {\n      \"description\": \"The dataset id\",\n      \"type\": \"integer\"\n    },\n    \"producing_tasks\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaskOutletDatasetReference\"\
  \n      },\n      \"type\": \"array\"\n    },\n    \"updated_at\": {\n      \"description\": \"The dataset update time\",\n      \"nullable\": false,\n      \"type\": \"string\"\n    },\n    \"uri\": {\n      \"description\": \"The dataset uri\",\n      \"nullable\": false,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dataset-schema.json
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
title: Dataset
---
