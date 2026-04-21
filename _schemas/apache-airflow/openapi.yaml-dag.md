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
