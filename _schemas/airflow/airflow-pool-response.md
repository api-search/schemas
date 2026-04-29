---
description: Pool serializer for responses.
layout: schema
name: PoolResponse
properties_list:
- description: ''
  name: name
  type: string
- description: Number of slots. Use -1 for unlimited.
  name: slots
  type: integer
- description: ''
  name: description
  type: object
- description: ''
  name: include_deferred
  type: boolean
- description: ''
  name: occupied_slots
  type: integer
- description: ''
  name: running_slots
  type: integer
- description: ''
  name: queued_slots
  type: integer
- description: ''
  name: scheduled_slots
  type: integer
- description: ''
  name: open_slots
  type: integer
- description: ''
  name: deferred_slots
  type: integer
- description: ''
  name: team_name
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-pool-response-schema.json
slug: airflow-pool-response
source_filename: airflow-pool-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-pool-response-schema.json\",\n  \"title\": \"PoolResponse\",\n  \"description\": \"Pool serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    },\n    \"slots\": {\n      \"type\": \"integer\",\n      \"minimum\": -1.0,\n      \"title\": \"Slots\",\n      \"description\": \"Number of slots. Use -1 for unlimited.\"\n    },\n    \"description\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Description\"\n    },\n    \"include_deferred\": {\n      \"type\": \"boolean\",\n      \"title\": \"Include Deferred\"\n    },\n    \"occupied_slots\": {\n      \"type\": \"integer\",\n      \"title\": \"Occupied\
  \ Slots\"\n    },\n    \"running_slots\": {\n      \"type\": \"integer\",\n      \"title\": \"Running Slots\"\n    },\n    \"queued_slots\": {\n      \"type\": \"integer\",\n      \"title\": \"Queued Slots\"\n    },\n    \"scheduled_slots\": {\n      \"type\": \"integer\",\n      \"title\": \"Scheduled Slots\"\n    },\n    \"open_slots\": {\n      \"type\": \"integer\",\n      \"title\": \"Open Slots\"\n    },\n    \"deferred_slots\": {\n      \"type\": \"integer\",\n      \"title\": \"Deferred Slots\"\n    },\n    \"team_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Team Name\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"slots\",\n    \"include_deferred\",\n    \"occupied_slots\",\n    \"running_slots\",\n    \"queued_slots\",\n    \"scheduled_slots\",\n    \"open_slots\",\n    \"deferred_slots\",\n    \"team_name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-pool-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: PoolResponse
---
