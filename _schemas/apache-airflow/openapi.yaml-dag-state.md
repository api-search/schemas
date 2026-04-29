---
description: DAG State. *Changed in version 2.1.3*&#58; 'queued' is added as a possible value.
layout: schema
name: DagState
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-dag-state-schema.json
slug: openapi.yaml-dag-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-state-schema.json\",\n  \"title\": \"DagState\",\n  \"description\": \"DAG State.\\n\\n*Changed in version 2.1.3*&#58; 'queued' is added as a possible value.\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"queued\",\n    \"running\",\n    \"success\",\n    \"failed\"\n  ],\n  \"readOnly\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-state-schema.json
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
title: DagState
---
