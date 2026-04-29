---
description: Event Log Response.
layout: schema
name: EventLogResponse
properties_list:
- description: ''
  name: event_log_id
  type: integer
- description: ''
  name: when
  type: string
- description: ''
  name: dag_id
  type: object
- description: ''
  name: task_id
  type: object
- description: ''
  name: run_id
  type: object
- description: ''
  name: map_index
  type: object
- description: ''
  name: try_number
  type: object
- description: ''
  name: event
  type: string
- description: ''
  name: logical_date
  type: object
- description: ''
  name: owner
  type: object
- description: ''
  name: extra
  type: object
- description: ''
  name: dag_display_name
  type: object
- description: ''
  name: task_display_name
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-event-log-response-schema.json
slug: airflow-event-log-response
source_filename: airflow-event-log-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-event-log-response-schema.json\",\n  \"title\": \"EventLogResponse\",\n  \"description\": \"Event Log Response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"event_log_id\": {\n      \"type\": \"integer\",\n      \"title\": \"Event Log Id\"\n    },\n    \"when\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"When\"\n    },\n    \"dag_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Dag Id\"\n    },\n    \"task_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Task Id\"\n    },\n    \"run_id\": {\n      \"anyOf\": [\n        {\n\
  \          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Run Id\"\n    },\n    \"map_index\": {\n      \"anyOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Map Index\"\n    },\n    \"try_number\": {\n      \"anyOf\": [\n        {\n          \"type\": \"integer\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Try Number\"\n    },\n    \"event\": {\n      \"type\": \"string\",\n      \"title\": \"Event\"\n    },\n    \"logical_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Logical Date\"\n    },\n    \"owner\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\
  \n        }\n      ],\n      \"title\": \"Owner\"\n    },\n    \"extra\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Extra\"\n    },\n    \"dag_display_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Dag Display Name\"\n    },\n    \"task_display_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Task Display Name\"\n    }\n  },\n  \"required\": [\n    \"event_log_id\",\n    \"when\",\n    \"dag_id\",\n    \"task_id\",\n    \"run_id\",\n    \"map_index\",\n    \"try_number\",\n    \"event\",\n    \"logical_date\",\n    \"owner\",\n    \"extra\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-event-log-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: EventLogResponse
---
