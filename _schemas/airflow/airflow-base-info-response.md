---
description: Base info serializer for responses.
layout: schema
name: BaseInfoResponse
properties_list:
- description: ''
  name: status
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-base-info-response-schema.json
slug: airflow-base-info-response
source_filename: airflow-base-info-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-base-info-response-schema.json\",\n  \"title\": \"BaseInfoResponse\",\n  \"description\": \"Base info serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Status\"\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-base-info-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: BaseInfoResponse
---
