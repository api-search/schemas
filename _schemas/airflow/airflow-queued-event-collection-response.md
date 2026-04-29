---
description: Queued Event Collection serializer for responses.
layout: schema
name: QueuedEventCollectionResponse
properties_list:
- description: ''
  name: queued_events
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-queued-event-collection-response-schema.json
slug: airflow-queued-event-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-queued-event-collection-response-schema.json\",\n  \"title\": \"QueuedEventCollectionResponse\",\n  \"description\": \"Queued Event Collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queued_events\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/QueuedEventResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Queued Events\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"queued_events\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-queued-event-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: QueuedEventCollectionResponse
---
