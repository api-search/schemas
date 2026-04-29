---
description: ListDagRunsForm schema from Apache Airflow API
layout: schema
name: ListDagRunsForm
properties_list:
- description: Return objects with specific DAG IDs. The value can be repeated to retrieve multiple matching values (OR condition).
  name: dag_ids
  type: array
- description: Returns objects greater or equal the specified date. This can be combined with end_date_lte parameter to receive only the selected period.
  name: end_date_gte
  type: string
- description: Returns objects less than or equal to the specified date. This can be combined with end_date_gte parameter to receive only the selected period.
  name: end_date_lte
  type: string
- description: Returns objects greater or equal to the specified date. This can be combined with execution_date_lte key to receive only the selected period.
  name: execution_date_gte
  type: string
- description: Returns objects less than or equal to the specified date. This can be combined with execution_date_gte key to receive only the selected period.
  name: execution_date_lte
  type: string
- description: The name of the field to order the results by. Prefix a field name with `-` to reverse the sort order. *New in version 2.1.0*
  name: order_by
  type: string
- description: The numbers of items to return.
  name: page_limit
  type: integer
- description: The number of items to skip before starting to collect the result set.
  name: page_offset
  type: integer
- description: Returns objects greater or equal the specified date. This can be combined with start_date_lte key to receive only the selected period.
  name: start_date_gte
  type: string
- description: Returns objects less or equal the specified date. This can be combined with start_date_gte parameter to receive only the selected period
  name: start_date_lte
  type: string
- description: Return objects with specific states. The value can be repeated to retrieve multiple matching values (OR condition).
  name: states
  type: array
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-list-dag-runs-form-schema.json
slug: openapi.yaml-list-dag-runs-form
source_filename: openapi.yaml-list-dag-runs-form-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-list-dag-runs-form-schema.json\",\n  \"title\": \"ListDagRunsForm\",\n  \"description\": \"ListDagRunsForm schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_ids\": {\n      \"description\": \"Return objects with specific DAG IDs.\\nThe value can be repeated to retrieve multiple matching values (OR condition).\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"end_date_gte\": {\n      \"description\": \"Returns objects greater or equal the specified date.\\n\\nThis can be combined with end_date_lte parameter to receive only the selected period.\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"end_date_lte\": {\n      \"description\": \"Returns objects less than or\
  \ equal to the specified date.\\n\\nThis can be combined with end_date_gte parameter to receive only the selected period.\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"execution_date_gte\": {\n      \"description\": \"Returns objects greater or equal to the specified date.\\n\\nThis can be combined with execution_date_lte key to receive only the selected period.\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"execution_date_lte\": {\n      \"description\": \"Returns objects less than or equal to the specified date.\\n\\nThis can be combined with execution_date_gte key to receive only the selected period.\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"order_by\": {\n      \"description\": \"The name of the field to order the results by. Prefix a field name\\nwith `-` to reverse the sort order.\\n\\n*New in version 2.1.0*\\n\",\n      \"type\": \"string\"\n    },\n    \"page_limit\"\
  : {\n      \"default\": 100,\n      \"description\": \"The numbers of items to return.\",\n      \"minimum\": 1,\n      \"type\": \"integer\"\n    },\n    \"page_offset\": {\n      \"description\": \"The number of items to skip before starting to collect the result set.\",\n      \"minimum\": 0,\n      \"type\": \"integer\"\n    },\n    \"start_date_gte\": {\n      \"description\": \"Returns objects greater or equal the specified date.\\n\\nThis can be combined with start_date_lte key to receive only the selected period.\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"start_date_lte\": {\n      \"description\": \"Returns objects less or equal the specified date.\\n\\nThis can be combined with start_date_gte parameter to receive only the selected period\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"states\": {\n      \"description\": \"Return objects with specific states.\\nThe value can be repeated to retrieve multiple\
  \ matching values (OR condition).\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-list-dag-runs-form-schema.json
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
title: ListDagRunsForm
---
