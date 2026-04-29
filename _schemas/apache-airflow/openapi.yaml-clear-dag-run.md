---
description: ClearDagRun schema from Apache Airflow API
layout: schema
name: ClearDagRun
properties_list:
- description: If set, don't actually run this operation. The response will contain a list of task instances planned to be cleaned, but not modified in any way.
  name: dry_run
  type: boolean
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-clear-dag-run-schema.json
slug: openapi.yaml-clear-dag-run
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-clear-dag-run-schema.json\",\n  \"title\": \"ClearDagRun\",\n  \"description\": \"ClearDagRun schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dry_run\": {\n      \"default\": true,\n      \"description\": \"If set, don't actually run this operation. The response will contain a list of task instances\\nplanned to be cleaned, but not modified in any way.\\n\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-clear-dag-run-schema.json
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
title: ClearDagRun
---
