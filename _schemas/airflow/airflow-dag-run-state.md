---
description: All possible states that a DagRun can be in. These are "shared" with TaskInstanceState in some parts of the code, so please ensure that their values always match the ones with the same name in TaskInstanceState.
layout: schema
name: DagRunState
properties_list: []
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-run-state-schema.json
slug: airflow-dag-run-state
source_filename: airflow-dag-run-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-state-schema.json\",\n  \"title\": \"DagRunState\",\n  \"description\": \"All possible states that a DagRun can be in.\\n\\nThese are \\\"shared\\\" with TaskInstanceState in some parts of the code,\\nso please ensure that their values always match the ones with the\\nsame name in TaskInstanceState.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"queued\",\n    \"running\",\n    \"success\",\n    \"failed\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-state-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DagRunState
---
