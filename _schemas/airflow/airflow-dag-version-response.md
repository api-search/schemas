---
description: Dag Version serializer for responses.
layout: schema
name: DagVersionResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: version_number
  type: integer
- description: ''
  name: dag_id
  type: string
- description: ''
  name: bundle_name
  type: object
- description: ''
  name: bundle_version
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: dag_display_name
  type: string
- description: ''
  name: bundle_url
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dag-version-response-schema.json
slug: airflow-dag-version-response
source_filename: airflow-dag-version-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-version-response-schema.json\",\n  \"title\": \"DagVersionResponse\",\n  \"description\": \"Dag Version serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"title\": \"Id\"\n    },\n    \"version_number\": {\n      \"type\": \"integer\",\n      \"title\": \"Version Number\"\n    },\n    \"dag_id\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Id\"\n    },\n    \"bundle_name\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Bundle Name\"\n    },\n    \"bundle_version\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\":\
  \ \"null\"\n        }\n      ],\n      \"title\": \"Bundle Version\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Created At\"\n    },\n    \"dag_display_name\": {\n      \"type\": \"string\",\n      \"title\": \"Dag Display Name\"\n    },\n    \"bundle_url\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Bundle Url\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"version_number\",\n    \"dag_id\",\n    \"bundle_name\",\n    \"bundle_version\",\n    \"created_at\",\n    \"dag_display_name\",\n    \"bundle_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dag-version-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DagVersionResponse
---
