---
description: Health serializer for responses.
layout: schema
name: HealthInfoResponse
properties_list:
- description: ''
  name: metadatabase
  type: object
- description: ''
  name: scheduler
  type: object
- description: ''
  name: triggerer
  type: object
- description: ''
  name: dag_processor
  type: object
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-health-info-response-schema.json
slug: airflow-health-info-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-health-info-response-schema.json\",\n  \"title\": \"HealthInfoResponse\",\n  \"description\": \"Health serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadatabase\": {\n      \"$ref\": \"#/components/schemas/BaseInfoResponse\"\n    },\n    \"scheduler\": {\n      \"$ref\": \"#/components/schemas/SchedulerInfoResponse\"\n    },\n    \"triggerer\": {\n      \"$ref\": \"#/components/schemas/TriggererInfoResponse\"\n    },\n    \"dag_processor\": {\n      \"anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DagProcessorInfoResponse\"\n        },\n        {\n          \"type\": \"null\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"metadatabase\",\n    \"scheduler\",\n    \"triggerer\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-health-info-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: HealthInfoResponse
---
