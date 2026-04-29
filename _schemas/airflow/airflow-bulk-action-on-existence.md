---
description: Bulk Action to be taken if the entity already exists or not.
layout: schema
name: BulkActionOnExistence
properties_list: []
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-bulk-action-on-existence-schema.json
slug: airflow-bulk-action-on-existence
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-action-on-existence-schema.json\",\n  \"title\": \"BulkActionOnExistence\",\n  \"description\": \"Bulk Action to be taken if the entity already exists or not.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"fail\",\n    \"skip\",\n    \"overwrite\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-action-on-existence-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: BulkActionOnExistence
---
