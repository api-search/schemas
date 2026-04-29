---
description: Full representation of Variable
layout: schema
name: Variable
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-variable-schema.json
slug: openapi.yaml-variable
source_filename: openapi.yaml-variable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-variable-schema.json\",\n  \"title\": \"Variable\",\n  \"description\": \"Full representation of Variable\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/VariableCollectionItem\"\n    },\n    {\n      \"properties\": {\n        \"value\": {\n          \"type\": \"string\"\n        }\n      },\n      \"type\": \"object\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-variable-schema.json
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
title: Variable
---
