---
description: Job Collection Response.
layout: schema
name: JobCollectionResponse
properties_list:
- description: ''
  name: jobs
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-job-collection-response-schema.json
slug: airflow-job-collection-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-job-collection-response-schema.json\",\n  \"title\": \"JobCollectionResponse\",\n  \"description\": \"Job Collection Response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Jobs\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"jobs\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-job-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: JobCollectionResponse
---
