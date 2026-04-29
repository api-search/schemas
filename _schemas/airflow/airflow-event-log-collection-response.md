---
description: Event Log Collection Response.
layout: schema
name: EventLogCollectionResponse
properties_list:
- description: ''
  name: event_logs
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-event-log-collection-response-schema.json
slug: airflow-event-log-collection-response
source_filename: airflow-event-log-collection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-event-log-collection-response-schema.json\",\n  \"title\": \"EventLogCollectionResponse\",\n  \"description\": \"Event Log Collection Response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"event_logs\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EventLogResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Event Logs\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"event_logs\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-event-log-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: EventLogCollectionResponse
---
