---
description: TaskInstanceReferenceCollection schema from Apache Airflow API
layout: schema
name: TaskInstanceReferenceCollection
properties_list:
- description: ''
  name: task_instances
  type: array
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-task-instance-reference-collection-schema.json
slug: openapi.yaml-task-instance-reference-collection
source_filename: openapi.yaml-task-instance-reference-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-instance-reference-collection-schema.json\",\n  \"title\": \"TaskInstanceReferenceCollection\",\n  \"description\": \"TaskInstanceReferenceCollection schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"task_instances\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaskInstanceReference\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-instance-reference-collection-schema.json
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
title: TaskInstanceReferenceCollection
---
