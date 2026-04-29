---
description: DagProcessor info serializer for responses.
layout: schema
name: DagProcessorInfoResponse
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: latest_dag_processor_heartbeat
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-processor-info-response-schema.json
slug: airflow-dag-processor-info-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-processor-info-response-schema.json\",\n  \"title\": \"DagProcessorInfoResponse\",\n  \"description\": \"DagProcessor info serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Status\"\n    },\n    \"latest_dag_processor_heartbeat\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Latest Dag Processor Heartbeat\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"latest_dag_processor_heartbeat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-processor-info-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DagProcessorInfoResponse
---
