---
description: 'For details see: [airflow.models.BaseOperator](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/index.html#airflow.models.BaseOperator)'
layout: schema
name: Task
properties_list:
- description: ''
  name: class_ref
  type: object
- description: ''
  name: depends_on_past
  type: boolean
- description: ''
  name: downstream_task_ids
  type: array
- description: ''
  name: end_date
  type: string
- description: ''
  name: execution_timeout
  type: object
- description: ''
  name: extra_links
  type: array
- description: ''
  name: is_mapped
  type: boolean
- description: ''
  name: owner
  type: string
- description: ''
  name: pool
  type: string
- description: ''
  name: pool_slots
  type: number
- description: ''
  name: priority_weight
  type: number
- description: ''
  name: queue
  type: string
- description: ''
  name: retries
  type: number
- description: ''
  name: retry_delay
  type: object
- description: ''
  name: retry_exponential_backoff
  type: boolean
- description: ''
  name: start_date
  type: string
- description: ''
  name: sub_dag
  type: object
- description: ''
  name: task_id
  type: string
- description: ''
  name: template_fields
  type: array
- description: ''
  name: trigger_rule
  type: object
- description: ''
  name: ui_color
  type: object
- description: ''
  name: ui_fgcolor
  type: object
- description: ''
  name: wait_for_downstream
  type: boolean
- description: ''
  name: weight_rule
  type: object
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-task-schema.json
slug: openapi.yaml-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"For details see:\\n[airflow.models.BaseOperator](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/models/index.html#airflow.models.BaseOperator)\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"class_ref\": {\n      \"$ref\": \"#/components/schemas/ClassReference\"\n    },\n    \"depends_on_past\": {\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"downstream_task_ids\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"end_date\": {\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"execution_timeout\": {\n      \"$ref\"\
  : \"#/components/schemas/TimeDelta\",\n      \"nullable\": true\n    },\n    \"extra_links\": {\n      \"items\": {\n        \"properties\": {\n          \"class_ref\": {\n            \"$ref\": \"#/components/schemas/ClassReference\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"is_mapped\": {\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"owner\": {\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"pool\": {\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"pool_slots\": {\n      \"readOnly\": true,\n      \"type\": \"number\"\n    },\n    \"priority_weight\": {\n      \"readOnly\": true,\n      \"type\": \"number\"\n    },\n    \"queue\": {\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"retries\": {\n      \"readOnly\": true,\n      \"type\": \"number\"\n    },\n    \"retry_delay\": {\n\
  \      \"$ref\": \"#/components/schemas/TimeDelta\",\n      \"nullable\": true\n    },\n    \"retry_exponential_backoff\": {\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"start_date\": {\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"sub_dag\": {\n      \"$ref\": \"#/components/schemas/DAG\"\n    },\n    \"task_id\": {\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"template_fields\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"trigger_rule\": {\n      \"$ref\": \"#/components/schemas/TriggerRule\"\n    },\n    \"ui_color\": {\n      \"$ref\": \"#/components/schemas/Color\"\n    },\n    \"ui_fgcolor\": {\n      \"$ref\": \"#/components/schemas/Color\"\n    },\n    \"wait_for_downstream\": {\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"weight_rule\": {\n      \"$ref\": \"#/components/schemas/WeightRule\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-task-schema.json
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
title: Task
---
