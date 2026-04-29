---
description: Pool serializer for patch bodies.
layout: schema
name: PoolPatchBody
properties_list:
- description: ''
  name: pool
  type: object
- description: ''
  name: slots
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: include_deferred
  type: object
- description: ''
  name: team_name
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-pool-patch-body-schema.json
slug: airflow-pool-patch-body
source_filename: airflow-pool-patch-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-pool-patch-body-schema.json\",\n  \"title\": \"PoolPatchBody\",\n  \"description\": \"Pool serializer for patch bodies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pool\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Pool\"\n    },\n    \"slots\": {\n      \"anyOf\": [\n        {\n          \"type\": \"integer\",\n          \"minimum\": -1.0,\n          \"description\": \"Number of slots. Use -1 for unlimited.\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Slots\"\n    },\n    \"description\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n\
  \      \"title\": \"Description\"\n    },\n    \"include_deferred\": {\n      \"anyOf\": [\n        {\n          \"type\": \"boolean\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Include Deferred\"\n    },\n    \"team_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"maxLength\": 50\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Team Name\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-pool-patch-body-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: PoolPatchBody
---
