---
description: Schema for a collection of Human-in-the-loop details.
layout: schema
name: HITLDetailCollection
properties_list:
- description: ''
  name: hitl_details
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-hitl-detail-collection-schema.json
slug: airflow-hitl-detail-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-hitl-detail-collection-schema.json\",\n  \"title\": \"HITLDetailCollection\",\n  \"description\": \"Schema for a collection of Human-in-the-loop details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hitl_details\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HITLDetail\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Hitl Details\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"hitl_details\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-hitl-detail-collection-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: HITLDetailCollection
---
