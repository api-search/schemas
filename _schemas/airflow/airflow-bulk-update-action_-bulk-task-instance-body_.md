---
description: BulkUpdateAction_BulkTaskInstanceBody_ schema from Apache Airflow API
layout: schema
name: BulkUpdateAction_BulkTaskInstanceBody_
properties_list:
- description: The action to be performed on the entities.
  name: action
  type: string
- description: A list of entities to be updated.
  name: entities
  type: array
- description: A list of field names to update for each entity.Only these fields will be applied from the request body to the database model.Any extra fields provided will be ignored.
  name: update_mask
  type: object
- description: ''
  name: action_on_non_existence
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-bulk-update-action_-bulk-task-instance-body_-schema.json
slug: airflow-bulk-update-action_-bulk-task-instance-body_
source_filename: airflow-bulk-update-action_-bulk-task-instance-body_-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-update-action_-bulk-task-instance-body_-schema.json\",\n  \"title\": \"BulkUpdateAction_BulkTaskInstanceBody_\",\n  \"description\": \"BulkUpdateAction_BulkTaskInstanceBody_ schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"update\",\n      \"title\": \"Action\",\n      \"description\": \"The action to be performed on the entities.\"\n    },\n    \"entities\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BulkTaskInstanceBody\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Entities\",\n      \"description\": \"A list of entities to be updated.\"\n    },\n    \"update_mask\": {\n      \"anyOf\": [\n        {\n          \"items\": {\n            \"type\": \"string\"\n     \
  \     },\n          \"type\": \"array\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Update Mask\",\n      \"description\": \"A list of field names to update for each entity.Only these fields will be applied from the request body to the database model.Any extra fields provided will be ignored.\"\n    },\n    \"action_on_non_existence\": {\n      \"$ref\": \"#/components/schemas/BulkActionNotOnExistence\",\n      \"default\": \"fail\"\n    }\n  },\n  \"required\": [\n    \"action\",\n    \"entities\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-bulk-update-action_-bulk-task-instance-body_-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: BulkUpdateAction_BulkTaskInstanceBody_
---
