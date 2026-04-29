---
description: Response of updating a Human-in-the-loop detail.
layout: schema
name: HITLDetailResponse
properties_list:
- description: ''
  name: responded_by
  type: object
- description: ''
  name: responded_at
  type: string
- description: ''
  name: chosen_options
  type: array
- description: ''
  name: params_input
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-hitl-detail-response-schema.json
slug: airflow-hitl-detail-response
source_filename: airflow-hitl-detail-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-hitl-detail-response-schema.json\",\n  \"title\": \"HITLDetailResponse\",\n  \"description\": \"Response of updating a Human-in-the-loop detail.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"responded_by\": {\n      \"$ref\": \"#/components/schemas/HITLUser\"\n    },\n    \"responded_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Responded At\"\n    },\n    \"chosen_options\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"title\": \"Chosen Options\"\n    },\n    \"params_input\": {\n      \"additionalProperties\": true,\n      \"type\": \"object\",\n      \"title\": \"Params Input\"\n    }\n  },\n  \"required\": [\n    \"responded_by\",\n    \"responded_at\",\n    \"chosen_options\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-hitl-detail-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: HITLDetailResponse
---
