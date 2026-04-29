---
description: TaskInstance schema from Apache Airflow API
layout: schema
name: TaskInstance
properties_list:
- description: ''
  name: dag_id
  type: string
- description: The DagRun ID for this task instance *New in version 2.3.0*
  name: dag_run_id
  type: string
- description: ''
  name: duration
  type: number
- description: ''
  name: end_date
  type: string
- description: ''
  name: execution_date
  type: string
- description: ''
  name: executor_config
  type: string
- description: ''
  name: hostname
  type: string
- description: ''
  name: map_index
  type: integer
- description: ''
  name: max_tries
  type: integer
- description: Contains manually entered notes by the user about the TaskInstance. *New in version 2.5.0*
  name: note
  type: string
- description: '*Changed in version 2.1.1*&#58; Field becomes nullable.'
  name: operator
  type: string
- description: ''
  name: pid
  type: integer
- description: ''
  name: pool
  type: string
- description: ''
  name: pool_slots
  type: integer
- description: ''
  name: priority_weight
  type: integer
- description: ''
  name: queue
  type: string
- description: ''
  name: queued_when
  type: string
- description: JSON object describing rendered fields. *New in version 2.3.0*
  name: rendered_fields
  type: object
- description: ''
  name: sla_miss
  type: object
- description: ''
  name: start_date
  type: string
- description: ''
  name: state
  type: object
- description: ''
  name: task_id
  type: string
- description: ''
  name: trigger
  type: object
- description: ''
  name: triggerer_job
  type: object
- description: ''
  name: try_number
  type: integer
- description: ''
  name: unixname
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-task-instance-schema.json
slug: openapi.yaml-task-instance
source_filename: openapi.yaml-task-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-instance-schema.json\",\n  \"title\": \"TaskInstance\",\n  \"description\": \"TaskInstance schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"type\": \"string\"\n    },\n    \"dag_run_id\": {\n      \"description\": \"The DagRun ID for this task instance\\n\\n*New in version 2.3.0*\\n\",\n      \"type\": \"string\"\n    },\n    \"duration\": {\n      \"nullable\": true,\n      \"type\": \"number\"\n    },\n    \"end_date\": {\n      \"format\": \"datetime\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"execution_date\": {\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    },\n    \"executor_config\": {\n      \"type\": \"string\"\n    },\n    \"hostname\": {\n      \"type\": \"string\"\n  \
  \  },\n    \"map_index\": {\n      \"type\": \"integer\"\n    },\n    \"max_tries\": {\n      \"type\": \"integer\"\n    },\n    \"note\": {\n      \"description\": \"Contains manually entered notes by the user about the TaskInstance.\\n\\n*New in version 2.5.0*\\n\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"operator\": {\n      \"description\": \"*Changed in version 2.1.1*&#58; Field becomes nullable.\\n\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"pid\": {\n      \"nullable\": true,\n      \"type\": \"integer\"\n    },\n    \"pool\": {\n      \"type\": \"string\"\n    },\n    \"pool_slots\": {\n      \"type\": \"integer\"\n    },\n    \"priority_weight\": {\n      \"nullable\": true,\n      \"type\": \"integer\"\n    },\n    \"queue\": {\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"queued_when\": {\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"rendered_fields\": {\n      \"description\"\
  : \"JSON object describing rendered fields.\\n\\n*New in version 2.3.0*\\n\",\n      \"type\": \"object\"\n    },\n    \"sla_miss\": {\n      \"$ref\": \"#/components/schemas/SLAMiss\",\n      \"nullable\": true\n    },\n    \"start_date\": {\n      \"format\": \"datetime\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"$ref\": \"#/components/schemas/TaskState\",\n      \"nullable\": true\n    },\n    \"task_id\": {\n      \"type\": \"string\"\n    },\n    \"trigger\": {\n      \"$ref\": \"#/components/schemas/Trigger\",\n      \"nullable\": true\n    },\n    \"triggerer_job\": {\n      \"$ref\": \"#/components/schemas/Job\",\n      \"nullable\": true\n    },\n    \"try_number\": {\n      \"type\": \"integer\"\n    },\n    \"unixname\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-instance-schema.json
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
title: TaskInstance
---
