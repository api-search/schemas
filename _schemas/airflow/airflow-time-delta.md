---
description: TimeDelta can be used to interact with datetime.timedelta objects.
layout: schema
name: TimeDelta
properties_list:
- description: ''
  name: __type
  type: string
- description: ''
  name: days
  type: integer
- description: ''
  name: seconds
  type: integer
- description: ''
  name: microseconds
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-time-delta-schema.json
slug: airflow-time-delta
source_filename: airflow-time-delta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-time-delta-schema.json\",\n  \"title\": \"TimeDelta\",\n  \"description\": \"TimeDelta can be used to interact with datetime.timedelta objects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"__type\": {\n      \"type\": \"string\",\n      \"title\": \"Type\",\n      \"default\": \"TimeDelta\"\n    },\n    \"days\": {\n      \"type\": \"integer\",\n      \"title\": \"Days\"\n    },\n    \"seconds\": {\n      \"type\": \"integer\",\n      \"title\": \"Seconds\"\n    },\n    \"microseconds\": {\n      \"type\": \"integer\",\n      \"title\": \"Microseconds\"\n    }\n  },\n  \"required\": [\n    \"days\",\n    \"seconds\",\n    \"microseconds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-time-delta-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TimeDelta
---
