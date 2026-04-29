---
description: All possible states that a Task Instance can be in. Note that None is also allowed, so always use this in a type hint with Optional.
layout: schema
name: TaskInstanceState
properties_list: []
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-task-instance-state-schema.json
slug: airflow-task-instance-state
source_filename: airflow-task-instance-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-instance-state-schema.json\",\n  \"title\": \"TaskInstanceState\",\n  \"description\": \"All possible states that a Task Instance can be in.\\n\\nNote that None is also allowed, so always use this in a type hint with Optional.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"removed\",\n    \"scheduled\",\n    \"queued\",\n    \"running\",\n    \"success\",\n    \"restarting\",\n    \"failed\",\n    \"up_for_retry\",\n    \"up_for_reschedule\",\n    \"upstream_failed\",\n    \"skipped\",\n    \"deferred\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-instance-state-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TaskInstanceState
---
