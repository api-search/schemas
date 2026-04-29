---
description: Task scheduling dependencies collection serializer for responses.
layout: schema
name: TaskDependencyCollectionResponse
properties_list:
- description: ''
  name: dependencies
  type: array
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-task-dependency-collection-response-schema.json
slug: airflow-task-dependency-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-dependency-collection-response-schema.json\",\n  \"title\": \"TaskDependencyCollectionResponse\",\n  \"description\": \"Task scheduling dependencies collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dependencies\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaskDependencyResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Dependencies\"\n    }\n  },\n  \"required\": [\n    \"dependencies\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-dependency-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TaskDependencyCollectionResponse
---
