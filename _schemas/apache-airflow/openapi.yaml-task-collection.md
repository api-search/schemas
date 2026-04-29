---
description: Collection of tasks.
layout: schema
name: TaskCollection
properties_list:
- description: ''
  name: tasks
  type: array
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-task-collection-schema.json
slug: openapi.yaml-task-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-collection-schema.json\",\n  \"title\": \"TaskCollection\",\n  \"description\": \"Collection of tasks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tasks\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Task\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-collection-schema.json
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
title: TaskCollection
---
