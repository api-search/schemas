---
description: The status and the latest scheduler heartbeat.
layout: schema
name: SchedulerStatus
properties_list:
- description: The time the scheduler last do a heartbeat.
  name: latest_scheduler_heartbeat
  type: string
- description: ''
  name: status
  type: object
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-scheduler-status-schema.json
slug: openapi.yaml-scheduler-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-scheduler-status-schema.json\",\n  \"title\": \"SchedulerStatus\",\n  \"description\": \"The status and the latest scheduler heartbeat.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"latest_scheduler_heartbeat\": {\n      \"description\": \"The time the scheduler last do a heartbeat.\",\n      \"format\": \"datetime\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"$ref\": \"#/components/schemas/HealthStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-scheduler-status-schema.json
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
title: SchedulerStatus
---
