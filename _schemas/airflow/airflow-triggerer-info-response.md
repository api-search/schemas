---
description: Triggerer info serializer for responses.
layout: schema
name: TriggererInfoResponse
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: latest_triggerer_heartbeat
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-triggerer-info-response-schema.json
slug: airflow-triggerer-info-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-triggerer-info-response-schema.json\",\n  \"title\": \"TriggererInfoResponse\",\n  \"description\": \"Triggerer info serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Status\"\n    },\n    \"latest_triggerer_heartbeat\": {\n      \"anyOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ],\n      \"title\": \"Latest Triggerer Heartbeat\"\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"latest_triggerer_heartbeat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-triggerer-info-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: TriggererInfoResponse
---
