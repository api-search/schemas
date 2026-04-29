---
description: TaskInstanceHistory serializer for responses.
layout: schema
name: TaskInstanceHistoryResponse
properties_list:
- description: ''
  name: task_id
  type: string
- description: ''
  name: dag_id
  type: string
- description: ''
  name: dag_run_id
  type: string
- description: ''
  name: map_index
  type: integer
- description: ''
  name: start_date
  type: object
- description: ''
  name: end_date
  type: object
- description: ''
  name: duration
  type: object
- description: ''
  name: state
  type: object
- description: ''
  name: try_number
  type: integer
- description: ''
  name: max_tries
  type: integer
- description: ''
  name: task_display_name
  type: string
- description: ''
  name: dag_display_name
  type: string
- description: ''
  name: hostname
  type: object
- description: ''
  name: unixname
  type: object
- description: ''
  name: pool
  type: string
- description: ''
  name: pool_slots
  type: integer
- description: ''
  name: queue
  type: object
- description: ''
  name: priority_weight
  type: object
- description: ''
  name: operator
  type: object
- description: ''
  name: operator_name
  type: object
- description: ''
  name: queued_when
  type: object
- description: ''
  name: scheduled_when
  type: object
- description: ''
  name: pid
  type: object
- description: ''
  name: executor
  type: object
- description: ''
  name: executor_config
  type: string
- description: ''
  name: dag_version
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-task-instance-history-response-schema.json
slug: airflow-task-instance-history-response
source_filename: airflow-task-instance-history-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-instance-history-response-schema.json\",\n  \"title\": \"TaskInstanceHistoryResponse\",\n  \"description\": \"TaskInstanceHistory serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"task_id\": {\n      \"type\": \"string\",\n      \"title\": \"Task Id\"\n    },\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"dag_run_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Run Id\"\n    },\n    \"map_index\": {\n      \"type\": \"integer\",\n      \"title\": \"Map Index\"\n    },\n    \"start_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Start Date\"\n    },\n    \"\
  end_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"End Date\"\n    },\n    \"duration\": {\n      \"anyOf\": [\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Duration\"\n    },\n    \"state\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskInstanceState\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ]\n    },\n    \"try_number\": {\n      \"type\": \"integer\",\n      \"title\": \"Try Number\"\n    },\n    \"max_tries\": {\n      \"type\": \"integer\",\n      \"title\": \"Max Tries\"\n    },\n    \"task_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Task Display Name\"\n    },\n    \"dag_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Display\
  \ Name\"\n    },\n    \"hostname\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Hostname\"\n    },\n    \"unixname\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Unixname\"\n    },\n    \"pool\": {\n      \"type\": \"string\",\n      \"title\": \"Pool\"\n    },\n    \"pool_slots\": {\n      \"type\": \"integer\",\n      \"title\": \"Pool Slots\"\n    },\n    \"queue\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Queue\"\n    },\n    \"priority_weight\": {\n      \"anyOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Priority Weight\"\n    },\n    \"operator\"\
  : {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Operator\"\n    },\n    \"operator_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Operator Name\"\n    },\n    \"queued_when\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Queued When\"\n    },\n    \"scheduled_when\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Scheduled When\"\n    },\n    \"pid\": {\n      \"anyOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"type\": \"\
  null\"\n        }\n      ],\n      \"title\": \"Pid\"\n    },\n    \"executor\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Executor\"\n    },\n    \"executor_config\": {\n      \"type\": \"string\",\n      \"title\": \"Executor Config\"\n    },\n    \"dag_version\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DagVersionResponse\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"task_id\",\n    \"dag_id\",\n    \"dag_run_id\",\n    \"map_index\",\n    \"start_date\",\n    \"end_date\",\n    \"duration\",\n    \"state\",\n    \"try_number\",\n    \"max_tries\",\n    \"task_display_name\",\n    \"dag_display_name\",\n    \"hostname\",\n    \"unixname\",\n    \"pool\",\n    \"pool_slots\",\n    \"queue\",\n    \"priority_weight\",\n    \"operator\",\n    \"operator_name\",\n    \"\
  queued_when\",\n    \"scheduled_when\",\n    \"pid\",\n    \"executor\",\n    \"executor_config\",\n    \"dag_version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-task-instance-history-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TaskInstanceHistoryResponse
---
