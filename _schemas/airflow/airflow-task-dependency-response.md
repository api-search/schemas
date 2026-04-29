---
description: Task Dependency serializer for responses.
layout: schema
name: TaskDependencyResponse
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: reason
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-task-dependency-response-schema.json
slug: airflow-task-dependency-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-dependency-response-schema.json\",\n  \"title\": \"TaskDependencyResponse\",\n  \"description\": \"Task Dependency serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"title\": \"Reason\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"reason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-dependency-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TaskDependencyResponse
---
