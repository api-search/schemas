---
description: Full representation of the connection.
layout: schema
name: Connection
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-connection-schema.json
slug: openapi.yaml-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-connection-schema.json\",\n  \"title\": \"Connection\",\n  \"description\": \"Full representation of the connection.\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/ConnectionCollectionItem\"\n    },\n    {\n      \"properties\": {\n        \"extra\": {\n          \"description\": \"Other values that cannot be put into another field, e.g. RSA keys.\",\n          \"nullable\": true,\n          \"type\": \"string\"\n        },\n        \"password\": {\n          \"description\": \"Password of the connection.\",\n          \"format\": \"password\",\n          \"type\": \"string\",\n          \"writeOnly\": true\n        }\n      },\n      \"type\": \"object\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-connection-schema.json
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
title: Connection
---
