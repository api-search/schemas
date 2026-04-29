---
description: Variable Collection serializer for responses.
layout: schema
name: VariableCollectionResponse
properties_list:
- description: ''
  name: variables
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-variable-collection-response-schema.json
slug: airflow-variable-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-variable-collection-response-schema.json\",\n  \"title\": \"VariableCollectionResponse\",\n  \"description\": \"Variable Collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"variables\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/VariableResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Variables\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"variables\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-variable-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: VariableCollectionResponse
---
