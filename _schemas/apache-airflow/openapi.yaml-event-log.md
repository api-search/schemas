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
