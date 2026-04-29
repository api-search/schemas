---
description: DAG
layout: schema
name: DAG
properties_list:
- description: The ID of the DAG.
  name: dag_id
  type: string
- description: Default view of the DAG inside the webserver *New in version 2.3.0*
  name: default_view
  type: string
- description: User-provided DAG description, which can consist of several sentences or paragraphs that describe DAG contents.
  name: description
  type: string
- description: 'The key containing the encrypted path to the file. Encryption and decryption take place only on the server. This prevents the client from reading an non-DAG file. This also ensures API extensibility, '
  name: file_token
  type: string
- description: The absolute path to the file.
  name: fileloc
  type: string
- description: Whether the DAG has import errors *New in version 2.3.0*
  name: has_import_errors
  type: boolean
- description: Whether the DAG has task concurrency limits *New in version 2.3.0*
  name: has_task_concurrency_limits
  type: boolean
- description: Whether the DAG is currently seen by the scheduler(s). *New in version 2.1.1* *Changed in version 2.2.0*&#58; Field is read-only.
  name: is_active
  type: boolean
- description: Whether the DAG is paused.
  name: is_paused
  type: boolean
- description: Whether the DAG is SubDAG.
  name: is_subdag
  type: boolean
- description: Time when the DAG last received a refresh signal (e.g. the DAG's "refresh" button was clicked in the web UI) *New in version 2.3.0*
  name: last_expired
  type: string
- description: The last time the DAG was parsed. *New in version 2.3.0*
  name: last_parsed_time
  type: string
- description: The last time the DAG was pickled. *New in version 2.3.0*
  name: last_pickled
  type: string
- description: Maximum number of active DAG runs for the DAG *New in version 2.3.0*
  name: max_active_runs
  type: integer
- description: Maximum number of active tasks that can be run on the DAG *New in version 2.3.0*
  name: max_active_tasks
  type: integer
- description: The logical date of the next dag run. *New in version 2.3.0*
  name: next_dagrun
  type: string
- description: Earliest time at which this ``next_dagrun`` can be created. *New in version 2.3.0*
  name: next_dagrun_create_after
  type: string
- description: The end of the interval of the next dag run. *New in version 2.3.0*
  name: next_dagrun_data_interval_end
  type: string
- description: The start of the interval of the next dag run. *New in version 2.3.0*
  name: next_dagrun_data_interval_start
  type: string
- description: ''
  name: owners
  type: array
- description: Foreign key to the latest pickle_id *New in version 2.3.0*
  name: pickle_id
  type: string
- description: If the DAG is SubDAG then it is the top level DAG identifier. Otherwise, null.
  name: root_dag_id
  type: string
- description: ''
  name: schedule_interval
  type: object
- description: Whether (one of) the scheduler is scheduling this DAG at the moment *New in version 2.3.0*
  name: scheduler_lock
  type: boolean
- description: List of tags.
  name: tags
  type: array
- description: Timetable/Schedule Interval description. *New in version 2.3.0*
  name: timetable_description
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-dag-schema.json
slug: openapi.yaml-dag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-schema.json\",\n  \"title\": \"DAG\",\n  \"description\": \"DAG\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"description\": \"The ID of the DAG.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"default_view\": {\n      \"description\": \"Default view of the DAG inside the webserver\\n\\n*New in version 2.3.0*\\n\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"User-provided DAG description, which can consist of several sentences or paragraphs that describe DAG contents.\\n\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"file_token\": {\n      \"description\": \"The key containing the encrypted\
  \ path to the file. Encryption and decryption take place only on the server. This prevents the client from reading an non-DAG file. This also ensures API extensibility, because the format of encrypted data may change.\\n\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"fileloc\": {\n      \"description\": \"The absolute path to the file.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"has_import_errors\": {\n      \"description\": \"Whether the DAG has import errors\\n\\n*New in version 2.3.0*\\n\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"has_task_concurrency_limits\": {\n      \"description\": \"Whether the DAG has task concurrency limits\\n\\n*New in version 2.3.0*\\n\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"is_active\": {\n      \"description\": \"Whether the DAG is currently seen by the scheduler(s).\\n\\n*New in version\
  \ 2.1.1*\\n\\n*Changed in version 2.2.0*&#58; Field is read-only.\\n\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"is_paused\": {\n      \"description\": \"Whether the DAG is paused.\",\n      \"nullable\": true,\n      \"type\": \"boolean\"\n    },\n    \"is_subdag\": {\n      \"description\": \"Whether the DAG is SubDAG.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"last_expired\": {\n      \"description\": \"Time when the DAG last received a refresh signal\\n(e.g. the DAG's \\\"refresh\\\" button was clicked in the web UI)\\n\\n*New in version 2.3.0*\\n\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"last_parsed_time\": {\n      \"description\": \"The last time the DAG was parsed.\\n\\n*New in version 2.3.0*\\n\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\"\
  : \"string\"\n    },\n    \"last_pickled\": {\n      \"description\": \"The last time the DAG was pickled.\\n\\n*New in version 2.3.0*\\n\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"max_active_runs\": {\n      \"description\": \"Maximum number of active DAG runs for the DAG\\n\\n*New in version 2.3.0*\\n\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"max_active_tasks\": {\n      \"description\": \"Maximum number of active tasks that can be run on the DAG\\n\\n*New in version 2.3.0*\\n\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"next_dagrun\": {\n      \"description\": \"The logical date of the next dag run.\\n\\n*New in version 2.3.0*\\n\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"next_dagrun_create_after\"\
  : {\n      \"description\": \"Earliest time at which this ``next_dagrun`` can be created.\\n\\n*New in version 2.3.0*\\n\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"next_dagrun_data_interval_end\": {\n      \"description\": \"The end of the interval of the next dag run.\\n\\n*New in version 2.3.0*\\n\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"next_dagrun_data_interval_start\": {\n      \"description\": \"The start of the interval of the next dag run.\\n\\n*New in version 2.3.0*\\n\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"owners\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"pickle_id\": {\n      \"description\": \"Foreign key to the\
  \ latest pickle_id\\n\\n*New in version 2.3.0*\\n\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"root_dag_id\": {\n      \"description\": \"If the DAG is SubDAG then it is the top level DAG identifier. Otherwise, null.\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"schedule_interval\": {\n      \"$ref\": \"#/components/schemas/ScheduleInterval\"\n    },\n    \"scheduler_lock\": {\n      \"description\": \"Whether (one of) the scheduler is scheduling this DAG at the moment\\n\\n*New in version 2.3.0*\\n\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"tags\": {\n      \"description\": \"List of tags.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Tag\"\n      },\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"timetable_description\": {\n      \"description\": \"Timetable/Schedule\
  \ Interval description.\\n\\n*New in version 2.3.0*\\n\",\n      \"nullable\": true,\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-schema.json
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
title: DAG
---
