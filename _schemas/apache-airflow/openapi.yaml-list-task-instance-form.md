---
description: ListTaskInstanceForm schema from Apache Airflow API
layout: schema
name: ListTaskInstanceForm
properties_list:
- description: Return objects with specific DAG IDs. The value can be repeated to retrieve multiple matching values (OR condition).
  name: dag_ids
  type: array
- description: Returns objects greater than or equal to the specified values. This can be combined with duration_lte parameter to receive only the selected period.
  name: duration_gte
  type: number
- description: Returns objects less than or equal to the specified values. This can be combined with duration_gte parameter to receive only the selected range.
  name: duration_lte
  type: number
- description: Returns objects greater or equal the specified date. This can be combined with start_date_lte parameter to receive only the selected period.
  name: end_date_gte
  type: string
- description: Returns objects less than or equal to the specified date. This can be combined with start_date_gte parameter to receive only the selected period.
  name: end_date_lte
  type: string
- description: Returns objects greater or equal to the specified date. This can be combined with execution_date_lte parameter to receive only the selected period.
  name: execution_date_gte
  type: string
- description: Returns objects less than or equal to the specified date. This can be combined with execution_date_gte parameter to receive only the selected period.
  name: execution_date_lte
  type: string
- description: The value can be repeated to retrieve multiple matching values (OR condition).
  name: pool
  type: array
- description: The value can be repeated to retrieve multiple matching values (OR condition).
  name: queue
  type: array
- description: Returns objects greater or equal the specified date. This can be combined with start_date_lte parameter to receive only the selected period.
  name: start_date_gte
  type: string
- description: Returns objects less or equal the specified date. This can be combined with start_date_gte parameter to receive only the selected period.
  name: start_date_lte
  type: string
- description: The value can be repeated to retrieve multiple matching values (OR condition).
  name: state
  type: array
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-list-task-instance-form-schema.json
slug: openapi.yaml-list-task-instance-form
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-list-task-instance-form-schema.json\",\n  \"title\": \"ListTaskInstanceForm\",\n  \"description\": \"ListTaskInstanceForm schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_ids\": {\n      \"description\": \"Return objects with specific DAG IDs.\\nThe value can be repeated to retrieve multiple matching values (OR condition).\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"duration_gte\": {\n      \"description\": \"Returns objects greater than or equal to the specified values.\\n\\nThis can be combined with duration_lte parameter to receive only the selected period.\\n\",\n      \"type\": \"number\"\n    },\n    \"duration_lte\": {\n      \"description\": \"Returns objects less than or equal to\
  \ the specified values.\\n\\nThis can be combined with duration_gte parameter to receive only the selected range.\\n\",\n      \"type\": \"number\"\n    },\n    \"end_date_gte\": {\n      \"description\": \"Returns objects greater or equal the specified date.\\n\\nThis can be combined with start_date_lte parameter to receive only the selected period.\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"end_date_lte\": {\n      \"description\": \"Returns objects less than or equal to the specified date.\\n\\nThis can be combined with start_date_gte parameter to receive only the selected period.\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"execution_date_gte\": {\n      \"description\": \"Returns objects greater or equal to the specified date.\\n\\nThis can be combined with execution_date_lte parameter to receive only the selected period.\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"\
  execution_date_lte\": {\n      \"description\": \"Returns objects less than or equal to the specified date.\\n\\nThis can be combined with execution_date_gte parameter to receive only the selected period.\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"pool\": {\n      \"description\": \"The value can be repeated to retrieve multiple matching values (OR condition).\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"queue\": {\n      \"description\": \"The value can be repeated to retrieve multiple matching values (OR condition).\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"start_date_gte\": {\n      \"description\": \"Returns objects greater or equal the specified date.\\n\\nThis can be combined with start_date_lte parameter to receive only the selected period.\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n \
  \   \"start_date_lte\": {\n      \"description\": \"Returns objects less or equal the specified date.\\n\\nThis can be combined with start_date_gte parameter to receive only the selected period.\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"description\": \"The value can be repeated to retrieve multiple matching values (OR condition).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaskState\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-list-task-instance-form-schema.json
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
title: ListTaskInstanceForm
---
