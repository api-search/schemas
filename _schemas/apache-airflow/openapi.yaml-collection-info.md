---
description: Metadata about collection.
layout: schema
name: CollectionInfo
properties_list:
- description: Count of total objects in the current result set before pagination parameters (limit, offset) are applied.
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-collection-info-schema.json
slug: openapi.yaml-collection-info
source_filename: openapi.yaml-collection-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-collection-info-schema.json\",\n  \"title\": \"CollectionInfo\",\n  \"description\": \"Metadata about collection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total_entries\": {\n      \"description\": \"Count of total objects in the current result set before pagination parameters\\n(limit, offset) are applied.\\n\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-collection-info-schema.json
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
title: CollectionInfo
---
