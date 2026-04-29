---
description: A collection of plugin. *New in version 2.1.0*
layout: schema
name: PluginCollection
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-plugin-collection-schema.json
slug: openapi.yaml-plugin-collection
source_filename: openapi.yaml-plugin-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-plugin-collection-schema.json\",\n  \"title\": \"PluginCollection\",\n  \"description\": \"A collection of plugin.\\n\\n*New in version 2.1.0*\\n\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"properties\": {\n        \"plugins\": {\n          \"items\": {\n            \"$ref\": \"#/components/schemas/PluginCollectionItem\"\n          },\n          \"type\": \"array\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/CollectionInfo\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-plugin-collection-schema.json
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
title: PluginCollection
---
