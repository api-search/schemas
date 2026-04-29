---
description: Schema for a Human-in-the-loop users.
layout: schema
name: HITLUser
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-hitl-user-schema.json
slug: airflow-hitl-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-hitl-user-schema.json\",\n  \"title\": \"HITLUser\",\n  \"description\": \"Schema for a Human-in-the-loop users.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"title\": \"Id\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-hitl-user-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: HITLUser
---
