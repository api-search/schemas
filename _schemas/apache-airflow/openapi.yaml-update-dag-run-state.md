---
description: Modify the state of a DAG run. *New in version 2.2.0*
layout: schema
name: UpdateDagRunState
properties_list:
- description: The state to set this DagRun
  name: state
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-update-dag-run-state-schema.json
slug: openapi.yaml-update-dag-run-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-update-dag-run-state-schema.json\",\n  \"title\": \"UpdateDagRunState\",\n  \"description\": \"Modify the state of a DAG run.\\n\\n*New in version 2.2.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"description\": \"The state to set this DagRun\",\n      \"enum\": [\n        \"success\",\n        \"failed\",\n        \"queued\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-update-dag-run-state-schema.json
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
title: UpdateDagRunState
---
