---
description: Collection of DAG warnings.
layout: schema
name: DagWarningCollection
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-dag-warning-collection-schema.json
slug: openapi.yaml-dag-warning-collection
source_filename: openapi.yaml-dag-warning-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-warning-collection-schema.json\",\n  \"title\": \"DagWarningCollection\",\n  \"description\": \"Collection of DAG warnings.\\n\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"properties\": {\n        \"import_errors\": {\n          \"items\": {\n            \"$ref\": \"#/components/schemas/DagWarning\"\n          },\n          \"type\": \"array\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/CollectionInfo\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-dag-warning-collection-schema.json
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
title: DagWarningCollection
---
