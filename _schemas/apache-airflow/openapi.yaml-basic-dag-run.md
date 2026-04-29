---
description: BasicDAGRun schema from Apache Airflow API
layout: schema
name: BasicDAGRun
properties_list:
- description: ''
  name: dag_id
  type: string
- description: ''
  name: data_interval_end
  type: string
- description: ''
  name: data_interval_start
  type: string
- description: ''
  name: end_date
  type: string
- description: The logical date (previously called execution date). This is the time or interval covered by this DAG run, according to the DAG definition. The value of this field can be set only when creating the ob
  name: logical_date
  type: string
- description: Run ID.
  name: run_id
  type: string
- description: The start time. The time when DAG run was actually created. *Changed in version 2.1.3*&#58; Field becomes nullable.
  name: start_date
  type: string
- description: ''
  name: state
  type: object
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-basic-dag-run-schema.json
slug: openapi.yaml-basic-dag-run
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-basic-dag-run-schema.json\",\n  \"title\": \"BasicDAGRun\",\n  \"description\": \"BasicDAGRun schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"data_interval_end\": {\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"data_interval_start\": {\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"end_date\": {\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"logical_date\": {\n      \"description\": \"The logical date (previously called execution\
  \ date). This is the time or interval covered by\\nthis DAG run, according to the DAG definition.\\n\\nThe value of this field can be set only when creating the object. If you try to modify the\\nfield of an existing object, the request fails with an BAD_REQUEST error.\\n\\nThis together with DAG_ID are a unique key.\\n\\n*New in version 2.2.0*\\n\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"run_id\": {\n      \"description\": \"Run ID.\\n\",\n      \"type\": \"string\"\n    },\n    \"start_date\": {\n      \"description\": \"The start time. The time when DAG run was actually created.\\n\\n*Changed in version 2.1.3*&#58; Field becomes nullable.\\n\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"$ref\": \"#/components/schemas/DagState\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-basic-dag-run-schema.json
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
title: BasicDAGRun
---
