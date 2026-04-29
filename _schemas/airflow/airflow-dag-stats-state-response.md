---
description: DagStatsState serializer for responses.
layout: schema
name: DagStatsStateResponse
properties_list:
- description: ''
  name: state
  type: object
- description: ''
  name: count
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-stats-state-response-schema.json
slug: airflow-dag-stats-state-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-stats-state-response-schema.json\",\n  \"title\": \"DagStatsStateResponse\",\n  \"description\": \"DagStatsState serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"$ref\": \"#/components/schemas/DagRunState\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"title\": \"Count\"\n    }\n  },\n  \"required\": [\n    \"state\",\n    \"count\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-stats-state-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DagStatsStateResponse
---
