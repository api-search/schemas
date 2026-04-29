---
description: DagRun serializer for asset responses.
layout: schema
name: DagRunAssetReference
properties_list:
- description: ''
  name: run_id
  type: string
- description: ''
  name: dag_id
  type: string
- description: ''
  name: logical_date
  type: object
- description: ''
  name: start_date
  type: string
- description: ''
  name: end_date
  type: object
- description: ''
  name: state
  type: string
- description: ''
  name: data_interval_start
  type: object
- description: ''
  name: data_interval_end
  type: object
- description: ''
  name: partition_key
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-run-asset-reference-schema.json
slug: airflow-dag-run-asset-reference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-asset-reference-schema.json\",\n  \"title\": \"DagRunAssetReference\",\n  \"description\": \"DagRun serializer for asset responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"run_id\": {\n      \"type\": \"string\",\n      \"title\": \"Run Id\"\n    },\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"logical_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Logical Date\"\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Start Date\"\n    },\n    \"end_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\
  ,\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"End Date\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"title\": \"State\"\n    },\n    \"data_interval_start\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Data Interval Start\"\n    },\n    \"data_interval_end\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Data Interval End\"\n    },\n    \"partition_key\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Partition Key\"\n    }\n  },\n  \"required\": [\n    \"run_id\",\n    \"\
  dag_id\",\n    \"logical_date\",\n    \"start_date\",\n    \"end_date\",\n    \"state\",\n    \"data_interval_start\",\n    \"data_interval_end\",\n    \"partition_key\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-run-asset-reference-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DagRunAssetReference
---
