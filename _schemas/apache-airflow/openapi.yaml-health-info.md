---
description: Instance status information.
layout: schema
name: HealthInfo
properties_list:
- description: ''
  name: metadatabase
  type: object
- description: ''
  name: scheduler
  type: object
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-health-info-schema.json
slug: openapi.yaml-health-info
source_filename: openapi.yaml-health-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-health-info-schema.json\",\n  \"title\": \"HealthInfo\",\n  \"description\": \"Instance status information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadatabase\": {\n      \"$ref\": \"#/components/schemas/MetadatabaseStatus\"\n    },\n    \"scheduler\": {\n      \"$ref\": \"#/components/schemas/SchedulerStatus\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-health-info-schema.json
tags:
- Apache
- DAG
- Data Pipeline
- ETL
- Open Source
- Orchestration
- Python
- Scheduling
- Workflow
title: HealthInfo
---
