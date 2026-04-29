---
description: Trigger serializer for responses.
layout: schema
name: TriggerResponse
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: classpath
  type: string
- description: ''
  name: kwargs
  type: string
- description: ''
  name: created_date
  type: string
- description: ''
  name: queue
  type: object
- description: ''
  name: triggerer_id
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-trigger-response-schema.json
slug: airflow-trigger-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-trigger-response-schema.json\",\n  \"title\": \"TriggerResponse\",\n  \"description\": \"Trigger serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"title\": \"Id\"\n    },\n    \"classpath\": {\n      \"type\": \"string\",\n      \"title\": \"Classpath\"\n    },\n    \"kwargs\": {\n      \"type\": \"string\",\n      \"title\": \"Kwargs\"\n    },\n    \"created_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Created Date\"\n    },\n    \"queue\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Queue\"\n    },\n    \"triggerer_id\": {\n      \"anyOf\": [\n        {\n       \
  \   \"type\": \"integer\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Triggerer Id\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"classpath\",\n    \"kwargs\",\n    \"created_date\",\n    \"queue\",\n    \"triggerer_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-trigger-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TriggerResponse
---
