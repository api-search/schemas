---
description: Last asset event response serializer.
layout: schema
name: LastAssetEventResponse
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: timestamp
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-last-asset-event-response-schema.json
slug: airflow-last-asset-event-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-last-asset-event-response-schema.json\",\n  \"title\": \"LastAssetEventResponse\",\n  \"description\": \"Last asset event response serializer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"anyOf\": [\n        {\n          \"type\": \"integer\",\n          \"minimum\": 0.0\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Id\"\n    },\n    \"timestamp\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-last-asset-event-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: LastAssetEventResponse
---
