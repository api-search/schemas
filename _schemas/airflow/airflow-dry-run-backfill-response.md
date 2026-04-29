---
description: Backfill serializer for responses in dry-run mode.
layout: schema
name: DryRunBackfillResponse
properties_list:
- description: ''
  name: logical_date
  type: object
- description: ''
  name: partition_key
  type: object
- description: ''
  name: partition_date
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-dry-run-backfill-response-schema.json
slug: airflow-dry-run-backfill-response
source_filename: airflow-dry-run-backfill-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dry-run-backfill-response-schema.json\",\n  \"title\": \"DryRunBackfillResponse\",\n  \"description\": \"Backfill serializer for responses in dry-run mode.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logical_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Logical Date\"\n    },\n    \"partition_key\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Partition Key\"\n    },\n    \"partition_date\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n     \
  \     \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Partition Date\"\n    }\n  },\n  \"required\": [\n    \"logical_date\",\n    \"partition_key\",\n    \"partition_date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-dry-run-backfill-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: DryRunBackfillResponse
---
