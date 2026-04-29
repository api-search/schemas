---
description: A user object with sensitive data. *New in version 2.1.0*
layout: schema
name: User
properties_list: []
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-user-schema.json
slug: openapi.yaml-user
source_filename: openapi.yaml-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-user-schema.json\",\n  \"title\": \"User\",\n  \"description\": \"A user object with sensitive data.\\n\\n*New in version 2.1.0*\\n\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/UserCollectionItem\"\n    },\n    {\n      \"properties\": {\n        \"password\": {\n          \"type\": \"string\",\n          \"writeOnly\": true\n        }\n      },\n      \"type\": \"object\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-user-schema.json
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
title: User
---
