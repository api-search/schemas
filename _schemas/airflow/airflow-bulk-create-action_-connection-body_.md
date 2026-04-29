---
description: BulkCreateAction_ConnectionBody_ schema from Apache Airflow API
layout: schema
name: BulkCreateAction_ConnectionBody_
properties_list:
- description: The action to be performed on the entities.
  name: action
  type: string
- description: A list of entities to be created.
  name: entities
  type: array
- description: ''
  name: action_on_existence
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-bulk-create-action_-connection-body_-schema.json
slug: airflow-bulk-create-action_-connection-body_
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-create-action_-connection-body_-schema.json\",\n  \"title\": \"BulkCreateAction_ConnectionBody_\",\n  \"description\": \"BulkCreateAction_ConnectionBody_ schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"create\",\n      \"title\": \"Action\",\n      \"description\": \"The action to be performed on the entities.\"\n    },\n    \"entities\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConnectionBody\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Entities\",\n      \"description\": \"A list of entities to be created.\"\n    },\n    \"action_on_existence\": {\n      \"$ref\": \"#/components/schemas/BulkActionOnExistence\",\n      \"default\": \"fail\"\n    }\n  },\n  \"required\"\
  : [\n    \"action\",\n    \"entities\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-create-action_-connection-body_-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: BulkCreateAction_ConnectionBody_
---
