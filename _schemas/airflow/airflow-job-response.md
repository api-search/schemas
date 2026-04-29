---
description: Job serializer for responses.
layout: schema
name: JobResponse
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: dag_id
  type: object
- description: ''
  name: state
  type: object
- description: ''
  name: job_type
  type: object
- description: ''
  name: start_date
  type: object
- description: ''
  name: end_date
  type: object
- description: ''
  name: latest_heartbeat
  type: object
- description: ''
  name: executor_class
  type: object
- description: ''
  name: hostname
  type: object
- description: ''
  name: unixname
  type: object
- description: ''
  name: dag_display_name
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-job-response-schema.json
slug: airflow-job-response
source_filename: airflow-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-job-response-schema.json\",\n  \"title\": \"JobResponse\",\n  \"description\": \"Job serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"title\": \"Id\"\n    },\n    \"dag_id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Dag Id\"\n    },\n    \"state\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"State\"\n    },\n    \"job_type\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Job Type\"\n\
  \    },\n    \"start_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Start Date\"\n    },\n    \"end_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"End Date\"\n    },\n    \"latest_heartbeat\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Latest Heartbeat\"\n    },\n    \"executor_class\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Executor Class\"\n    },\n    \"hostname\": {\n      \"anyOf\": [\n        {\n    \
  \      \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Hostname\"\n    },\n    \"unixname\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Unixname\"\n    },\n    \"dag_display_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Dag Display Name\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"dag_id\",\n    \"state\",\n    \"job_type\",\n    \"start_date\",\n    \"end_date\",\n    \"latest_heartbeat\",\n    \"executor_class\",\n    \"hostname\",\n    \"unixname\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-job-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: JobResponse
---
