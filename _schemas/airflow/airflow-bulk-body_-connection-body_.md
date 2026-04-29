---
description: BulkBody_ConnectionBody_ schema from Apache Airflow API
layout: schema
name: BulkBody_ConnectionBody_
properties_list:
- description: ''
  name: actions
  type: array
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-bulk-body_-connection-body_-schema.json
slug: airflow-bulk-body_-connection-body_
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-body_-connection-body_-schema.json\",\n  \"title\": \"BulkBody_ConnectionBody_\",\n  \"description\": \"BulkBody_ConnectionBody_ schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actions\": {\n      \"items\": {\n        \"oneOf\": [\n          {\n            \"$ref\": \"#/components/schemas/BulkCreateAction_ConnectionBody_\"\n          },\n          {\n            \"$ref\": \"#/components/schemas/BulkUpdateAction_ConnectionBody_\"\n          },\n          {\n            \"$ref\": \"#/components/schemas/BulkDeleteAction_ConnectionBody_\"\n          }\n        ]\n      },\n      \"type\": \"array\",\n      \"title\": \"Actions\"\n    }\n  },\n  \"required\": [\n    \"actions\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-body_-connection-body_-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: BulkBody_ConnectionBody_
---
