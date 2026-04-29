---
description: a role item. *New in version 2.1.0*
layout: schema
name: Role
properties_list:
- description: ''
  name: actions
  type: array
- description: The name of the role *Changed in version 2.3.0*&#58; A minimum character length requirement ('minLength') is added.
  name: name
  type: string
provider_name: Apache Airflow
provider_slug: apache-airflow
schema_file: json-schema/openapi.yaml-role-schema.json
slug: openapi.yaml-role
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-role-schema.json\",\n  \"title\": \"Role\",\n  \"description\": \"a role item.\\n\\n*New in version 2.1.0*\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actions\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ActionResource\"\n      },\n      \"type\": \"array\"\n    },\n    \"name\": {\n      \"description\": \"The name of the role\\n\\n*Changed in version 2.3.0*&#58; A minimum character length requirement ('minLength') is added.\\n\",\n      \"minLength\": 1,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-airflow/refs/heads/main/json-schema/openapi.yaml-role-schema.json
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
title: Role
---
