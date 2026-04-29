---
description: Collection of providers. *New in version 2.1.0*
layout: schema
name: ProviderCollection
properties_list:
- description: ''
  name: providers
  type: array
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-provider-collection-schema.json
slug: openapi.yaml-provider-collection
source_filename: openapi.yaml-provider-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-provider-collection-schema.json\",\n  \"title\": \"ProviderCollection\",\n  \"description\": \"Collection of providers.\\n\\n*New in version 2.1.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"providers\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Provider\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-provider-collection-schema.json
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
title: ProviderCollection
---
