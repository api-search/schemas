---
description: Asset serializer for responses.
layout: schema
name: AssetResponse
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: uri
  type: string
- description: ''
  name: group
  type: string
- description: ''
  name: extra
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: scheduled_dags
  type: array
- description: ''
  name: producing_tasks
  type: array
- description: ''
  name: consuming_tasks
  type: array
- description: ''
  name: aliases
  type: array
- description: ''
  name: watchers
  type: array
- description: ''
  name: last_asset_event
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-asset-response-schema.json
slug: airflow-asset-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-response-schema.json\",\n  \"title\": \"AssetResponse\",\n  \"description\": \"Asset serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"title\": \"Id\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"title\": \"Name\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"title\": \"Uri\"\n    },\n    \"group\": {\n      \"type\": \"string\",\n      \"title\": \"Group\"\n    },\n    \"extra\": {\n      \"anyOf\": [\n        {\n          \"additionalProperties\": {\n            \"$ref\": \"#/components/schemas/JsonValue\"\n          },\n          \"type\": \"object\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Extra\"\n    },\n    \"created_at\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Created At\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"title\": \"Updated At\"\n    },\n    \"scheduled_dags\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DagScheduleAssetReference\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Scheduled Dags\"\n    },\n    \"producing_tasks\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaskOutletAssetReference\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Producing Tasks\"\n    },\n    \"consuming_tasks\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TaskInletAssetReference\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Consuming Tasks\"\n    },\n    \"aliases\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AssetAliasResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Aliases\"\
  \n    },\n    \"watchers\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AssetWatcherResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Watchers\"\n    },\n    \"last_asset_event\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastAssetEventResponse\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"uri\",\n    \"group\",\n    \"created_at\",\n    \"updated_at\",\n    \"scheduled_dags\",\n    \"producing_tasks\",\n    \"consuming_tasks\",\n    \"aliases\",\n    \"watchers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-asset-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: AssetResponse
---
