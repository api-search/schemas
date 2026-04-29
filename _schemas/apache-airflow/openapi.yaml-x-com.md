---
description: Full representations of XCom entry.
layout: schema
name: XCom
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-x-com-schema.json
slug: openapi.yaml-x-com
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-x-com-schema.json\",\n  \"title\": \"XCom\",\n  \"description\": \"Full representations of XCom entry.\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/XComCollectionItem\"\n    },\n    {\n      \"properties\": {\n        \"value\": {\n          \"description\": \"The value\",\n          \"type\": \"string\"\n        }\n      },\n      \"type\": \"object\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-x-com-schema.json
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
title: XCom
---
