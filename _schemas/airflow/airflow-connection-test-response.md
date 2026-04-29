---
description: Connection Test serializer for responses.
layout: schema
name: ConnectionTestResponse
properties_list:
- description: ''
  name: status
  type: boolean
- description: ''
  name: message
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-connection-test-response-schema.json
slug: airflow-connection-test-response
source_filename: airflow-connection-test-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-connection-test-response-schema.json\",\n  \"title\": \"ConnectionTestResponse\",\n  \"description\": \"Connection Test serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"boolean\",\n      \"title\": \"Status\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"title\": \"Message\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-connection-test-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ConnectionTestResponse
---
