---
description: Provider Collection serializer for responses.
layout: schema
name: ProviderCollectionResponse
properties_list:
- description: ''
  name: providers
  type: array
- description: ''
  name: total_entries
  type: integer
provider_name: Apache Airflow
provider_slug: airflow
schema_file: json-schema/airflow-provider-collection-response-schema.json
slug: airflow-provider-collection-response
source_filename: airflow-provider-collection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-provider-collection-response-schema.json\",\n  \"title\": \"ProviderCollectionResponse\",\n  \"description\": \"Provider Collection serializer for responses.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"providers\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ProviderResponse\"\n      },\n      \"type\": \"array\",\n      \"title\": \"Providers\"\n    },\n    \"total_entries\": {\n      \"type\": \"integer\",\n      \"title\": \"Total Entries\"\n    }\n  },\n  \"required\": [\n    \"providers\",\n    \"total_entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airflow/refs/heads/main/json-schema/airflow-provider-collection-response-schema.json
tags:
- Workflow Orchestration
- Data Pipeline
- Open Source
- Apache
- DAG
- Scheduling
- ETL
- Data Engineering
title: ProviderCollectionResponse
---
