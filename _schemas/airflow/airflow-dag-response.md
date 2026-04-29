---
description: DAG serializer for responses.
layout: schema
name: DAGResponse
properties_list:
- description: ''
  name: dag_id
  type: string
- description: ''
  name: dag_display_name
  type: string
- description: ''
  name: is_paused
  type: boolean
- description: ''
  name: is_stale
  type: boolean
- description: ''
  name: last_parsed_time
  type: object
- description: ''
  name: last_parse_duration
  type: object
- description: ''
  name: last_expired
  type: object
- description: ''
  name: bundle_name
  type: object
- description: ''
  name: bundle_version
  type: object
- description: ''
  name: relative_fileloc
  type: object
- description: ''
  name: fileloc
  type: string
- description: ''
  name: description
  type: object
- description: ''
  name: timetable_summary
  type: object
- description: ''
  name: timetable_description
  type: object
- description: ''
  name: timetable_partitioned
  type: boolean
- description: ''
  name: timetable_periodic
  type: boolean
- description: ''
  name: tags
  type: array
- description: ''
  name: max_active_tasks
  type: integer
- description: ''
  name: max_active_runs
  type: object
- description: ''
  name: max_consecutive_failed_dag_runs
  type: integer
- description: ''
  name: has_task_concurrency_limits
  type: boolean
- description: ''
  name: has_import_errors
  type: boolean
- description: ''
  name: next_dagrun_logical_date
  type: object
- description: ''
  name: next_dagrun_data_interval_start
  type: object
- description: ''
  name: next_dagrun_data_interval_end
  type: object
- description: ''
  name: next_dagrun_run_after
  type: object
- description: ''
  name: allowed_run_types
  type: object
- description: ''
  name: owners
  type: array
- description: Whether this DAG's schedule supports backfilling.
  name: is_backfillable
  type: boolean
- description: Return file token.
  name: file_token
  type: string
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-response-schema.json
slug: airflow-dag-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-response-schema.json\",\n  \"title\": \"DAGResponse\",\n  \"description\": \"DAG serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"dag_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Display Name\"\n    },\n    \"is_paused\": {\n      \"type\": \"boolean\",\n      \"title\": \"Is Paused\"\n    },\n    \"is_stale\": {\n      \"type\": \"boolean\",\n      \"title\": \"Is Stale\"\n    },\n    \"last_parsed_time\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Last Parsed Time\"\n    },\n    \"last_parse_duration\":\
  \ {\n      \"anyOf\": [\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Last Parse Duration\"\n    },\n    \"last_expired\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Last Expired\"\n    },\n    \"bundle_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Bundle Name\"\n    },\n    \"bundle_version\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Bundle Version\"\n    },\n    \"relative_fileloc\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n       \
  \ }\n      ],\n      \"title\": \"Relative Fileloc\"\n    },\n    \"fileloc\": {\n      \"type\": \"string\",\n      \"title\": \"Fileloc\"\n    },\n    \"description\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Description\"\n    },\n    \"timetable_summary\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Timetable Summary\"\n    },\n    \"timetable_description\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Timetable Description\"\n    },\n    \"timetable_partitioned\": {\n      \"type\": \"boolean\",\n      \"title\": \"Timetable Partitioned\"\n    },\n    \"timetable_periodic\": {\n      \"type\": \"boolean\",\n      \"title\": \"Timetable Periodic\"\
  \n    },\n    \"tags\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DagTagResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Tags\"\n    },\n    \"max_active_tasks\": {\n      \"type\": \"integer\",\n      \"title\": \"Max Active Tasks\"\n    },\n    \"max_active_runs\": {\n      \"anyOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Max Active Runs\"\n    },\n    \"max_consecutive_failed_dag_runs\": {\n      \"type\": \"integer\",\n      \"title\": \"Max Consecutive Failed Dag Runs\"\n    },\n    \"has_task_concurrency_limits\": {\n      \"type\": \"boolean\",\n      \"title\": \"Has Task Concurrency Limits\"\n    },\n    \"has_import_errors\": {\n      \"type\": \"boolean\",\n      \"title\": \"Has Import Errors\"\n    },\n    \"next_dagrun_logical_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\
  \n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Next Dagrun Logical Date\"\n    },\n    \"next_dagrun_data_interval_start\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Next Dagrun Data Interval Start\"\n    },\n    \"next_dagrun_data_interval_end\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Next Dagrun Data Interval End\"\n    },\n    \"next_dagrun_run_after\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Next Dagrun Run After\"\n    },\n    \"allowed_run_types\": {\n      \"anyOf\": [\n\
  \        {\n          \"items\": {\n            \"$ref\": \"#/components/schemas/DagRunType\"\n          },\n          \"type\": \"array\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Allowed Run Types\"\n    },\n    \"owners\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Owners\"\n    },\n    \"is_backfillable\": {\n      \"type\": \"boolean\",\n      \"title\": \"Is Backfillable\",\n      \"description\": \"Whether this DAG's schedule supports backfilling.\",\n      \"readOnly\": true\n    },\n    \"file_token\": {\n      \"type\": \"string\",\n      \"title\": \"File Token\",\n      \"description\": \"Return file token.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"dag_id\",\n    \"dag_display_name\",\n    \"is_paused\",\n    \"is_stale\",\n    \"last_parsed_time\",\n    \"last_parse_duration\",\n    \"last_expired\",\n    \"bundle_name\",\n    \"\
  bundle_version\",\n    \"relative_fileloc\",\n    \"fileloc\",\n    \"description\",\n    \"timetable_summary\",\n    \"timetable_description\",\n    \"timetable_partitioned\",\n    \"timetable_periodic\",\n    \"tags\",\n    \"max_active_tasks\",\n    \"max_active_runs\",\n    \"max_consecutive_failed_dag_runs\",\n    \"has_task_concurrency_limits\",\n    \"has_import_errors\",\n    \"next_dagrun_logical_date\",\n    \"next_dagrun_data_interval_start\",\n    \"next_dagrun_data_interval_end\",\n    \"next_dagrun_run_after\",\n    \"allowed_run_types\",\n    \"owners\",\n    \"is_backfillable\",\n    \"file_token\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DAGResponse
---
