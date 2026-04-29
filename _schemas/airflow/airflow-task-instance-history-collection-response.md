---
description: TaskInstanceHistory Collection serializer for responses.
layout: schema
name: TaskInstanceHistoryCollectionResponse
properties_list:
- description: ''
  name: task_instances
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-task-instance-history-collection-response-schema.json
slug: airflow-task-instance-history-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-instance-history-collection-response-schema.json\",\n  \"title\": \"TaskInstanceHistoryCollectionResponse\",\n  \"description\": \"TaskInstanceHistory Collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"task_instances\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaskInstanceHistoryResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Task Instances\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"task_instances\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-instance-history-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TaskInstanceHistoryCollectionResponse
---
