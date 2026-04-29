---
description: The pool
layout: schema
name: Pool
properties_list:
- description: The description of the pool. *New in version 2.3.0*
  name: description
  type: string
- description: The name of pool.
  name: name
  type: string
- description: The number of slots used by running/queued tasks at the moment.
  name: occupied_slots
  type: integer
- description: The number of free slots at the moment.
  name: open_slots
  type: integer
- description: The number of slots used by queued tasks at the moment.
  name: queued_slots
  type: integer
- description: The maximum number of slots that can be assigned to tasks. One job may occupy one or more slots.
  name: slots
  type: integer
- description: The number of slots used by running tasks at the moment.
  name: used_slots
  type: integer
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-pool-schema.json
slug: openapi.yaml-pool
source_filename: openapi.yaml-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-pool-schema.json\",\n  \"title\": \"Pool\",\n  \"description\": \"The pool\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"The description of the pool.\\n\\n*New in version 2.3.0*\\n\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of pool.\",\n      \"type\": \"string\"\n    },\n    \"occupied_slots\": {\n      \"description\": \"The number of slots used by running/queued tasks at the moment.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"open_slots\": {\n      \"description\": \"The number of free slots at the moment.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"queued_slots\": {\n      \"description\": \"The number\
  \ of slots used by queued tasks at the moment.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"slots\": {\n      \"description\": \"The maximum number of slots that can be assigned to tasks. One job may occupy one or more slots.\\n\",\n      \"type\": \"integer\"\n    },\n    \"used_slots\": {\n      \"description\": \"The number of slots used by running tasks at the moment.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-pool-schema.json
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
title: Pool
---
