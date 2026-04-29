---
description: The status of the metadatabase.
layout: schema
name: MetadatabaseStatus
properties_list:
- description: ''
  name: status
  type: object
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-metadatabase-status-schema.json
slug: openapi.yaml-metadatabase-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-metadatabase-status-schema.json\",\n  \"title\": \"MetadatabaseStatus\",\n  \"description\": \"The status of the metadatabase.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"$ref\": \"#/components/schemas/HealthStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-metadatabase-status-schema.json
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
title: MetadatabaseStatus
---
