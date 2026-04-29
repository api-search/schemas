---
description: DAGRun schema from Apache Airflow API
layout: schema
name: DAGRun
properties_list:
- description: JSON object describing additional configuration parameters. The value of this field can be set only when creating the object. If you try to modify the field of an existing object, the request fails wi
  name: conf
  type: object
- description: ''
  name: dag_id
  type: string
- description: Run ID. The value of this field can be set only when creating the object. If you try to modify the field of an existing object, the request fails with an BAD_REQUEST error. If not provided, a value wi
  name: dag_run_id
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
- description: The execution date. This is the same as logical_date, kept for backwards compatibility. If both this field and logical_date are provided but with different values, the request will fail with an BAD_RE
  name: execution_date
  type: string
- description: ''
  name: external_trigger
  type: boolean
- description: ''
  name: last_scheduling_decision
  type: string
- description: The logical date (previously called execution date). This is the time or interval covered by this DAG run, according to the DAG definition. The value of this field can be set only when creating the ob
  name: logical_date
  type: string
- description: Contains manually entered notes by the user about the DagRun. *New in version 2.5.0*
  name: note
  type: string
- description: ''
  name: run_type
  type: string
- description: The start time. The time when DAG run was actually created. *Changed in version 2.1.3*&#58; Field becomes nullable.
  name: start_date
  type: string
- description: ''
  name: state
  type: object
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-dag-run-schema.json
slug: openapi.yaml-dag-run
source_filename: openapi.yaml-dag-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-run-schema.json\",\n  \"title\": \"DAGRun\",\n  \"description\": \"DAGRun schema from Apache Airflow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conf\": {\n      \"description\": \"JSON object describing additional configuration parameters.\\n\\nThe value of this field can be set only when creating the object. If you try to modify the\\nfield of an existing object, the request fails with an BAD_REQUEST error.\\n\",\n      \"type\": \"object\"\n    },\n    \"dag_id\": {\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"dag_run_id\": {\n      \"description\": \"Run ID.\\n\\nThe value of this field can be set only when creating the object. If you try to modify the\\nfield of an existing object, the request fails with an BAD_REQUEST error.\\n\\nIf not provided,\
  \ a value will be generated based on execution_date.\\n\\nIf the specified dag_run_id is in use, the creation request fails with an ALREADY_EXISTS error.\\n\\nThis together with DAG_ID are a unique key.\\n\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"data_interval_end\": {\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"data_interval_start\": {\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"end_date\": {\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"execution_date\": {\n      \"deprecated\": true,\n      \"description\": \"The execution date. This is the same as logical_date, kept for backwards compatibility.\\nIf both this field and logical_date are provided but with different values, the request\\nwill fail with\
  \ an BAD_REQUEST error.\\n\\n*Changed in version 2.2.0*&#58; Field becomes nullable.\\n\\n*Deprecated since version 2.2.0*&#58; Use 'logical_date' instead.\\n\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"external_trigger\": {\n      \"default\": true,\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"last_scheduling_decision\": {\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"logical_date\": {\n      \"description\": \"The logical date (previously called execution date). This is the time or interval covered by\\nthis DAG run, according to the DAG definition.\\n\\nThe value of this field can be set only when creating the object. If you try to modify the\\nfield of an existing object, the request fails with an BAD_REQUEST error.\\n\\nThis together with DAG_ID are a unique key.\\n\\n*New in version 2.2.0*\\n\",\n      \"format\"\
  : \"date-time\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"note\": {\n      \"description\": \"Contains manually entered notes by the user about the DagRun.\\n\\n*New in version 2.5.0*\\n\",\n      \"nullable\": true,\n      \"type\": \"string\"\n    },\n    \"run_type\": {\n      \"enum\": [\n        \"backfill\",\n        \"manual\",\n        \"scheduled\",\n        \"dataset_triggered\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"start_date\": {\n      \"description\": \"The start time. The time when DAG run was actually created.\\n\\n*Changed in version 2.1.3*&#58; Field becomes nullable.\\n\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"$ref\": \"#/components/schemas/DagState\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-run-schema.json
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
title: DAGRun
---
