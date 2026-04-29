---
description: Class with DagRun types.
layout: schema
name: DagRunType
properties_list: []
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-run-type-schema.json
slug: airflow-dag-run-type
source_filename: airflow-dag-run-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-type-schema.json\",\n  \"title\": \"DagRunType\",\n  \"description\": \"Class with DagRun types.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"backfill\",\n    \"scheduled\",\n    \"manual\",\n    \"operator_triggered\",\n    \"asset_triggered\",\n    \"asset_materialization\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-type-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DagRunType
---
