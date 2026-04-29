---
description: Schema for Human-in-the-loop detail.
layout: schema
name: HITLDetail
properties_list:
- description: ''
  name: options
  type: array
- description: ''
  name: subject
  type: string
- description: ''
  name: body
  type: object
- description: ''
  name: defaults
  type: object
- description: ''
  name: multiple
  type: boolean
- description: ''
  name: params
  type: object
- description: ''
  name: assigned_users
  type: array
- description: ''
  name: created_at
  type: string
- description: ''
  name: responded_by_user
  type: object
- description: ''
  name: responded_at
  type: object
- description: ''
  name: chosen_options
  type: object
- description: ''
  name: params_input
  type: object
- description: ''
  name: response_received
  type: boolean
- description: ''
  name: task_instance
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-hitl-detail-schema.json
slug: airflow-hitl-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-hitl-detail-schema.json\",\n  \"title\": \"HITLDetail\",\n  \"description\": \"Schema for Human-in-the-loop detail.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"options\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"title\": \"Options\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"title\": \"Subject\"\n    },\n    \"body\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Body\"\n    },\n    \"defaults\": {\n      \"anyOf\": [\n        {\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"type\": \"array\"\n        },\n        {\n          \"type\": \"\
  null\"\n        }\n      ],\n      \"title\": \"Defaults\"\n    },\n    \"multiple\": {\n      \"type\": \"boolean\",\n      \"title\": \"Multiple\",\n      \"default\": false\n    },\n    \"params\": {\n      \"additionalProperties\": true,\n      \"type\": \"object\",\n      \"title\": \"Params\"\n    },\n    \"assigned_users\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HITLUser\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Assigned Users\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Created At\"\n    },\n    \"responded_by_user\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HITLUser\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ]\n    },\n    \"responded_at\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n    \
  \    }\n      ],\n      \"title\": \"Responded At\"\n    },\n    \"chosen_options\": {\n      \"anyOf\": [\n        {\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"type\": \"array\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Chosen Options\"\n    },\n    \"params_input\": {\n      \"additionalProperties\": true,\n      \"type\": \"object\",\n      \"title\": \"Params Input\"\n    },\n    \"response_received\": {\n      \"type\": \"boolean\",\n      \"title\": \"Response Received\",\n      \"default\": false\n    },\n    \"task_instance\": {\n      \"$ref\": \"#/components/schemas/TaskInstanceResponse\"\n    }\n  },\n  \"required\": [\n    \"options\",\n    \"subject\",\n    \"created_at\",\n    \"task_instance\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-hitl-detail-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: HITLDetail
---
