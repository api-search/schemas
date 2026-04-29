---
description: Log of user operations via CLI or Web UI.
layout: schema
name: EventLog
properties_list:
- description: The DAG ID
  name: dag_id
  type: string
- description: A key describing the type of event.
  name: event
  type: string
- description: The event log ID
  name: event_log_id
  type: integer
- description: When the event was dispatched for an object having execution_date, the value of this field.
  name: execution_date
  type: string
- description: Other information that was not included in the other fields, e.g. the complete CLI command.
  name: extra
  type: string
- description: Name of the user who triggered these events a.
  name: owner
  type: string
- description: The DAG ID
  name: task_id
  type: string
- description: The time when these events happened.
  name: when
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-event-log-schema.json
slug: openapi.yaml-event-log
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-event-log-schema.json\",\n  \"title\": \"EventLog\",\n  \"description\": \"Log of user operations via CLI or Web UI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"description\": \"The DAG ID\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"event\": {\n      \"description\": \"A key describing the type of event.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"event_log_id\": {\n      \"description\": \"The event log ID\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"execution_date\": {\n      \"description\": \"When the event was dispatched for an object having execution_date, the value of this field.\\n\",\n      \"format\": \"date-time\",\n      \"nullable\"\
  : true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"extra\": {\n      \"description\": \"Other information that was not included in the other fields, e.g. the complete CLI command.\\n\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"owner\": {\n      \"description\": \"Name of the user who triggered these events a.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"task_id\": {\n      \"description\": \"The DAG ID\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"when\": {\n      \"description\": \"The time when these events happened.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-event-log-schema.json
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
title: EventLog
---
