---
description: Schema for updating the content of a Human-in-the-loop detail.
layout: schema
name: UpdateHITLDetailPayload
properties_list:
- description: ''
  name: chosen_options
  type: array
- description: ''
  name: params_input
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-update-hitl-detail-payload-schema.json
slug: airflow-update-hitl-detail-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-update-hitl-detail-payload-schema.json\",\n  \"title\": \"UpdateHITLDetailPayload\",\n  \"description\": \"Schema for updating the content of a Human-in-the-loop detail.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"chosen_options\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"title\": \"Chosen Options\"\n    },\n    \"params_input\": {\n      \"additionalProperties\": true,\n      \"type\": \"object\",\n      \"title\": \"Params Input\"\n    }\n  },\n  \"required\": [\n    \"chosen_options\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-update-hitl-detail-payload-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: UpdateHITLDetailPayload
---
